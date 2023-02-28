---
layout: post
title:  "10 phím tắt giúp phát triển với Flutter trên VSCode nhanh hơn, hiệu quả hơn"
author: dantino
categories: [Flutter, Tham khảo]
image: assets/images/posts/flutter-vscode-shortcuts/flutter-vscode-shortcuts-banner.png
tags: []
toc: true
---
# Phát triển ứng dụng với Flutter trên Visual Studio Code (VSCode) - Nhanh hơn, hiệu quả hơn

VSCode là một ứng dụng được Microsoft phát triển, là một IDE tuyệt vời cho lập trình viên, đặt biệt với việc phát triển ứng dụng với Flutter.
Ngoài VSCode, để lập trình với Flutter và Dart, lập trình viên có thể sử dụng Android Studio hoặc IntelliJ.

VSCode được tôi sử dụng trong quá trình phát triển các dự án, do đó, trong tất cả các bài viết, tôi sẽ tập trung vào VSCode là môi trường phát triển chính.

Sau khi các bạn hoàn thành [cài đặt theo các bước hướng dẫn cơ bản][basic-setup-steps],việc tiếp theo để nâng cao hiệu suất quá trình làm việc là tìm hiểu và tối ưu quy trình làm việc.

Trong loạt bài về tối ưu và nâng cao hiệu suất làm việc với VSCode, tôi chia ra làm 2 phần:

**1. Các phím tắt**

**2. Các gói mở rộng (Extension)**

Trong bài viết này sẽ đề cập đến 10 phím tắt mà tôi sử dụng hàng ngày khi lập trình cho các dự án.

Bạn có thể tham khảo nhiều bài viết và video liên quan đến các Tips sử dụng VSCode, dưới đây là danh sách các phím tắt mà tôi thường dùng

![Tóm tắt 10 tiện ích mở rộng]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/10-shortcuts.png)



## Các phím tắt thưởng sử dụng 

### 1. Mở Command Palette
- MacOS: CMD+Shift+P
- Windows: CTRL+Shift+P
Khi nhấn tổ hợp phím này, VSCode sẽ mở ra của sổ để ta có thể thực hiện một số lệnh một cách nhanh chóng, như tạo dự án mới, thêm gói tích hợp vào dự án,...

![Mở Command Palette]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/01-show-command-palette.gif)

### 2. Fix lỗi nhanh (Quick Fix actions)

- MacOS: CMD + .
- Windows: CTRL + .

Bạn có thể thực hiện các lệnh nhanh như tạo Widget bao widget hiện tại (Wrap), tạo Widget con từ code được chọn, đổi vai trò (di chuyển widget được chọn thành parent)

Nội dung hiển thị tuỳ thuộc vào ngữ cảnh mà con trỏ đang có.  
Bạn nên thử nghiệm với nhiều tình huống khác nhau để nắm rõ hơn tổ hợp phím vạn năng này.


![Quick-Fix]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/02-quick-fix.png) 

### 3. Tìm kiếm file theo tên

- MacOS: CMD+P
- Windows: CTRL+P

Khi dự án lớn, có nhiều file, đôi khi gây khó khăn trong việc tìm ra vị trí của file trong thư mục dự án, vì vậy, tổ hợp phím này sẽ giúp bạn nhanh chóng tìm ra file cần thiết.

![Tìm file theo tên]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/03-search-files-by-name.png) 

### 4. Mở nhanh danh sách phím tắt

- MacOS: CMD+K+S
- Windows: CTRL+K+S

Số lượng phím tắt quá nhiều, trong khi bạn có nhiều thứ phải nhớ và bận tâm hàng ngày, đôi khi chúng ta cũng cần tham khảo thêm các phím tắt khác, bạn có thể mở danh sách các phím tắt với tổ hợp phím trên.

![Danh sách tổ hợp phím tắt]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/04-shorcut-list.png) 

### 5. Đổi tên (Rename Symbol) 

- MacOS: CMD+R+R
- Windows: CTRL+R+R

Khi muốn đổi tên biến, hàm, hoặc lớp (Class),... trong nhiều vị trí, nhiều file khác nhau, nếu đổi theo cách thủ công có thể chúng ta sẽ bỏ sót hoặc gây lỗi.
Vì vậy, tổ hợp phím trên rất có ích. giúp tiết kiệm thời gian và giảm các sai sót.

![Thay đổi tên]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/05-rename-symbol.gif) 


### 6. Nhân đôi dòng code (Duplicate line) 

- MacOS: CMD+C -> CMD + V
- Windows: CTRL+C -> CTRL + V

Ta có thể thực hiện theo cách thông thước là bôi dòng văn bản và chọn Copy/Paste; nhưng với tổ hợp phím trên, bạn không nhất thiết phải chọn hết text trên dòng, chỉ cần đặt con trỏ ở dòng cần nhân đôi.

![Nhân đôi dòng code]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/06-duplicate-quick-fix-code.gif) 

### 7. Xem định nghĩa code hoặc mã nguồn (View quick source code) 

 - CMD + Di chuyển chuột  hoặc click trải
 - CTRL + Di chuyển chuột  hoặc click trải

Tổ hợp phím này giúp quá trình lập trình, nếu có một số nội dung chưa hiểu về hàm, về class, có thể xem nhanh bằng cách nhấn tổ hợp phí trên.

![Xem nhanh code]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/07-show-code-hint.gif) 


### 8. Di chuyển code lên xuống

- Control + ↑ / ↓
- Alt + ↑ / ↓
  
![Xem nhanh code]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/08-move-code-up-down.gif) 



### 9. Ẩn hoặc hiện code (Comment / Uncomment) 

- MacOS: CMD + /
- Windows: CTRL + /

Tổ hợp phím giúp nhanh chóng đánh dấu code có sử dụng hay chỉ là dòng chú thích, code không sử dụng.
Trong quá trình debug code có thể phải sử dụng phím này để thử từng dòng hoặc cụm code.

![Comment - Umcomment]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/09-comment.gif) 

### 10. Tìm và thanh thế trong file

 - MacOS: CMD + F
 - Windows: CTRL + F

Tìm kiếm nhanh chóng trong file

![Tìm kiếm trong file]({{ site.baseurl }}/assets/images/posts/flutter-vscode-shortcuts/10-search-in-file.gif) 


Hy vọng các tổ hợp phím trên hữu ích trong quá trình bạn lập trình. Bạn có thể khám phá thêm nhiều tổ hợp phím khác cũng như các mẹo sử dụng VSCode như trong Link video ở cuối bài.


***Trong phần 2, chúng ta sẽ tìm hiểu thêm các gói mở rộng (Extension) trong VSCode sẽ giúp ích rất nhiều trong quá trình lập trình với Flutter.***

---
[Các Tips với VSCode - YouTube Video - Fireship.io](https://www.youtube.com/watch?v=ifTF3ags0XI)


---



[basic-setup-steps]: https://docs.flutter.dev/development/tools/vs-code
