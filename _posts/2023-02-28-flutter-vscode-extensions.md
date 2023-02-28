---
layout: post
title:  "10 tiện ích mở rộng giúp phát triển với Flutter trên VSCode nhanh hơn, hiệu quả hơn"
author: dantino
categories: [Flutter, Tham khảo]
image: assets/images/posts/flutter-vscode-extensions/flutter-vscode-extensions-banner.png
tags: []
toc: true
---

# 10 tiện ích mở rộng trên VSCode hỗ trợ phát triển Flutter và Dart

Trong loạt bài về tối ưu và nâng cao hiệu suất làm việc với VSCode, tôi chia ra làm 2 phần:

  [**1. Các phím tắt**][shortcuts]

  **2. Các gói mở rộng**

[Bài viết trước][shortcuts] chúng ta đã tìm hiểu 10 tổ hợp phím tắt hữu dụng.
Trong bài viết tiếp theo này sẽ đề cập đến 10 tiện ích mở rộng mà tôi sử dụng hàng ngày khi lập trình cho các dự án.

## [01. Dart Class Generator][dart-class-generator]

Với các Class dạng Data Model và có thể sử dụng với các dạng dữ liệu kiểu json, việc sử dụng tiện ích này rất hữu ích.

Bộ công cụ [Dart Class Generator][class-generator]

![Dart Class Generator]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/01-dart-class-generator.gif)

## [02. Dart Barrel File Generator][dart-barrel-file-generator]

Khi có nhiều file liên quan, khi sử dụng, có thể phải import nhiều file riêng lẻ, thay vì vậy, chúng ta có thể gọp lại thành 1 file tổng và có thể import để sử dụng.

Bộ công cụ Dart [Barrel File Generator][dart-barrel-file-generator] sẽ giúp tạo nhanh file này.

![Dart Barrel file Generator]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/02-dart-barrel-file-generator.gif)

## [03. Awesome Flutter Snippets][flutter-awesome-snippets]

Việc tạo file, import và tạp các widget chuẩn là việc thường xuyên trong quá trình lập trình với Flutter, với công cụ này, sẽ tiết kiệm được thời gian rất nhiều bằng việc tạo ra các đoạn code mẫu.

![Flutter Awesome Snippets]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/03-flutter-awesome-snippets.gif)

## [04. Flutter Riverpod Snippets][flutter-riverpod-snippets]

Nếu bạn sử dụng Riverpod trong quản lý trạng thái (State Management) thì tiện ích này cũng rất hữu ích, tương tự Flutter Awesome Snippets

![Riverpod Snippets]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/04-riverpod-snippets.gif)


## [05. Error Lens][error-lens]
Trong quá trình lập trình, có thể sẽ có những lỗi liên quan đến đánh máy, Error Lens sẽ giúp gây chú ý cho bạn để nhận ra các lỗi sai

![Error Lens]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/05-error-lens.png)

## [06. Version Lens][version-lens]

Trong dự án sử dụng nhiều package đi kèm, theo thời gian, các package này có thể đã lỗi thời, chúng ta có thể sử dụng Verson Lens để kiểm tra và cập nhật kịp thời.

![Version Lens]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/06-version-lens.gif)


## [07. Better Comments][better-comments]

Việc ghi chú trong quá trình lập trình rất quan trọng, giúp chúng ta lưu ý hoặc ghi chú một số nội dung quan trọng nào đó.
Do đó, Better Comments giúp tạo comment một cách nhanh chóng, dễ dàng với các từ khoá khác nhau như: NOTE, FIXME,...

![Better Comments]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/07-better-comments.png)

## [08. Comment Anchors][comment-anchors]

Cùng với Better Comments, Comment Anchors cũng giúp theo dõi các comment một cách nhanh chóng

![Better Comments]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/08-comment-anchors.gif)

## [09. Back & Forth][back-n-forth]

Khi mở file và thay đổi xem nội dung giữa các file, có thể chúng ta sẽ gặp khó khi muốn trở lại dòng lệnh trước trong file nào đó, Back & Forth giúp công việc này được trở nên nhẹ nhàng hơn.

![Back n Forth]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/09-back-and-forth.gif)

## [10. Firebase Explorer][firebase-explorer]

Nếu bạn thường xuyên làm việc với Firebase, thì đây là công cụ rất hữu ích
giúp bạn có thể xem này Firebase trong VSCode, không cần phải mở Firebase Console trên trình duyệt.

![Firebase Explorer]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/10-firebase-explorer.png)


File mindmap giới thiệu tổng thể các nội dung 2 bài viết về shortcuts và extensions

![mindmap shortcuts và extensions trên vscode]({{ site.baseurl }}/assets/images/posts/flutter-vscode-extensions/vscode-shortcuts-extensions-map.png)



---
[Các Tips với VSCode - YouTube Video - Fireship.io](https://www.youtube.com/watch?v=ifTF3ags0XI)


---




[basic-setup-steps]: https://docs.flutter.dev/development/tools/vs-code

[shortcuts]: https://flutteriot.com/flutter-vscode-shortcuts/

[dart-class-generator]: https://marketplace.visualstudio.com/items?itemName=hzgood.dart-data-class-generator

[dart-barrel-file-generator]: https://marketplace.visualstudio.com/items?itemName=miquelddg.dart-barrel-file-generator

[flutter-awesome-snippets]: https://marketplace.visualstudio.com/items?itemName=Nash.awesome-flutter-snippets

[flutter-riverpod-snippets]: https://marketplace.visualstudio.com/items?itemName=robert-brunhage.flutter-riverpod-snippets

[error-lens]: https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens

[version-lens]: https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens

[better-comments]: https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments

[comment-anchors]: https://marketplace.visualstudio.com/items?itemName=ExodiusStudios.comment-anchors

[back-n-forth]: https://marketplace.visualstudio.com/items?itemName=nick-rudenko.back-n-forth

[firebase-explorer]: https://marketplace.visualstudio.com/items?itemName=jsayol.firebase-explorer
