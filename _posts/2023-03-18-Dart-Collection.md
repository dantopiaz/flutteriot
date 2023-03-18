---
layout: post
title:  "Collection trong Dart"
author: dantino
categories: [Flutter]
image: assets/images/posts/dart-collections/dart-collections.png
tags: [featured]
toc: true
---
# Một số điểm lưu ý trong kiểu Collection trong ngôn ngữ lập trình Dart

## 1. Kiểu List

Trong ngôn ngữ lập trình Dart, không có kiểu dữ liệu dạng Array nhưng có dạng List.

```dart

    // Một số cách khai báo List<T>, trong đó T là kiểu dữ liệu
  
    // 1.  List of int
    final intList1 = [1,2,3]; // Trình biên dịch tự nhận dạng kiểu dữ liệu là số int
  
    // 2. empty list of int
    //Thêm kiểu biến trong dấu kép <>
    final intList2Fixed = <int>[];
  
    // 3. empty list of int
    final List<int> intList3 = [];
  
    intList1.add(4); // thêm phần tử 
    final len1 = intList1.length; // Lấy số phần tử trong list 
    print(len1); // Kết quả: 4
    intList1.clear() ;// Xoá list, trở thành list trống
    print(intList1.length); // kết quả: 0
```

Toán tử mở rộng ... có thể được sử dụng để copy 1 list
```dart
    // null list
    List<int>? nullList;
    //Copy và sử dụng toán tử mở rộng là: ... và ...? (kiểm tra null)
    intList3 = [...nullList]; // Error
    var list3 = [...?nullList]; // OK, có kiểm tra null, nullList chỉ được thêm vào nếu không null.
```

Bạn có thể đặt câu điều kiện trong List để thêm hoặc không thêm, ví dụ:
```dart
    final hasTopping = false;
  
    final drinks = [
        'Hồng trà',
        'Trà sen',
        if (hasTopping) 'Topping',
    ];
  
    print(drinks); //Kq: [Hồng trà, Trà sen]
```
Và:
```dart
    final hasTopping = true;
    
    final drinks = [
        'Hồng trà',
        'Trà sen',
        if (hasTopping) 'Topping',
    ];
    
    print(drinks); //Kq: [Hồng trà, Trà sen, Topping]
```
Trong trường hợp sử dụng const thay vì final, thì trình biên dịch sẽ càng tối hưu khi biên dịch:
```dart
    const hasTopping = true;
    
    final drinks = const [
        'Hồng trà',
        'Trà sen',
        if (hasTopping) 'Topping',
    ];

```
Bạn cũng có thể áp dụng tương tự cho for
```dart
// tạo list int từ 1->10
    final myNumber = [
        1,2,3,
        for (var i = 4; i <= 10; ++i) i
    ];
```

## 2. Kiểu Set 
Set<T> được sử dụng chứa các phần tử, trong đó, không có phần từ nào trùng lập.
Ví dụ:
```dart
    // List
    var intList  = [1,2,3,1,2,3]; // List of int, OK
    print(intList); // [1, 2, 3, 1, 2, 3]
    // Set
    var intSet = {1,2,3,1,2,3}; //  tự động loại các phần tử lặp lại
    print(intSet); // {1, 2, 3}
```
**Lưu ý khi khai báo kiểu Set**
```dart
    // 1. Xác định kiểu trực tiếp khi khai báo, int 
    Set<int> emptySet1 = {};
  
    // 2. Kiểu được đặt trước {}
    var emptySet2 = <int>{};
  
    // 3. Là Map, không phải Set. Nếu không xác định kiểu dữ liệu, trình biên dịch sẽ hiểu là Map dang dynamic
    final emptySet3 = {};
    
    emptySet1 = {1,2,3};
    emptySet2.addAll(emptySet1);
    print(emptySet2); //{1, 2, 3}
    emptySet2.addAll([4,5,6]); // thêm nhiều thành phần, thì phải đặt dạng mảng,[ ]
    print(emptySet2); // {1, 2, 3, 4, 5, 6}
    final set3 = {6,7,8};
    emptySet2 = {...set3};
    print(emptySet2); // {6, 7, 8}

```
Set<T> cũng hỗ trợ các toán tử ... và ...? như với List<T>; đồng thời bạn cũng có thể sử dụng if và for tương tự với List.



## 3. Kiểu Map

Còn được biết đến như dạng dictionary, Map<K,V> là dạng lưu dữ liệu theo kiểu key-value (từ khoá - giá trị)

Ví dụ:
```dart
    final Map<int, String>  m = {
        0: 'Trà sữa',
        1: 'Cafe',
        2: 'Nước ngọt',
    }
```
Bạn có thể sử dụng `putIfAbsent` để thêm phần từ vào map nếu chưa có trong map

```dart
    // Vì key = 0 đã tồn tại, nên sẽ KHÔNG thêm "Nước trái cây"
    m.putIfAbsent(0, () => 'Nước trái cây'); 

    // Vì key = 3 chưa tồn tại, nên sẽ  thêm "Nước trái cây"
    m.putIfAbsent(3, () => 'Nước trái cây'); 
``` 

Thêm hoặc cập nhật phần tử của map:
```dart
    // Nếu phần tử đã có, thì giá trị sẽ được cập nhật
    // Vị trí key = 0 là "Trà sữa" sẽ bị thay bằng "Trà đào"
    m[0] = 'Trà đào';

    // Nếu phần tử chưa có, giá trị sẽ được thêm vào
    // Key = 4 chưa có, nên "Trà đá" được thêm vào ở key = 4
    m[4] = 'Trà đá';
```

Truy cập phần tử của map:
```dart
    final mon = m[0] ; // mon = 'Trà sữa'
    final mon1 = m[5]; // mon1 = null, vì chưa có trong map 

    // Tốt nhất nên kiểm tra trước khi truy cập giá trị
    if (containKey(2) {
        print(m[2]) ; // 'Nước ngọt'
    }

```

## Lưu ý khi áp dụng

List có 2 hàm đang lưu ý khi sử dụng: `reduce()` và `fold()`

Cơ bản, 2 hàm này hoạt động tương tự nhau, nhưng `fold()` đòi hỏi giá trị bắt đầu
```dart
    final list = [1,2,3,4,5];
  
    // reduce((a,b) => c)
    final sum = list.reduce((a,b) => a + b);
    print(sum); // 15
  
    //fold(initValue, (a,b) => c)
    final sumFold1 = list.fold(0, (a,b) => a+b);
    final sumFold2 = list.fold(10, (a,b) => a+b);
    print(sumFold1); // 15
    print(sumFold2); // 25
```
Trong khi `reduce()` đòi hỏi cùng kiểu dữ liệu
```dart
    T reduce(
        T combine(T value, T element)
) 
```

Thì `fold()` cho phép 2 kiểu dữ liệu khác nhau
```dart
    T fold(
    T initialValue,
    T combine(T previousValue, E element)
) 
```

Ví dụ: 
```dart
    final str = ['Welcome', 'to', 'Flutter'];
    final sumStr = str.reduce((String a, String b) => a + b);
    print(sumStr); // WelcometoFlutter
  
    //Lỗi vì reduce đòi hỏi cùng kiểu dữ liệu
    final sumStr2 = str.reduce((String a, String b) => a.length + b.length);
  
    // fold cho  phép trên các kiểu dữ liệu khác nhau
    final int sumStrFold = str.fold<int>(0, (int count, String b) => count+ b.length);
    print(sumStrFold); // 16
```

Để hiểu rõ hơn và thử các nội dung trên, bạn có thể sử dụng [DartPad](https://dartpad.dev).
