# blender_ui - Giao Diện Người Dùng của Blender trong Tiếng Việt
Đây là đề án phiên dịch giao diện phần mềm nguồn mở 
[Blender](https://www.blender.org/download/) sang tiếng Việt. 
Các bạn có thể lấy bản 
[blender.mo](https://github.com/hoangduytran/blender_ui/blob/main/3x/blender.mo) này về máy và nạp vào thư mục tương ứng (xem dưới đây) để có thể đổi giao diện phần mềm sang tiếng Việt và sử dụng nó trong ngôn ngữ mẹ đẻ của mình. 
Đương nhiên, bản này hiện cũng đang trên đà được tiến hành, và hằng ngày sẽ có bản cập nhật các thay đổi mới nhất.
Mong các bạn để ý ngày và giờ xuất xưởng mà tôi đăng lên đây để xem và lấy bản mới nhất về máy.

Sau khi lấy xuống máy thì đưa vào thư mục của phần mềm trên máy bằng cách mở một cửa sổ dòng lệnh và đánh dòng lệnh ví dụ sau đây, tùy theo hệ điều hành mà bạn sử dụng:

Tôi sử dụng phiên bản 2.93 trong các ví dụ dưới đây. Nếu bạn sử dụng 3.0 hoặc 3.1 chẳng hạn, thì thay giá trị 2.93 bằng 3.0 hoặc 3.1 nhé. Đường dẫn cơ bản là từ thư mục 'datafiles'. Các bạn phải có thư mục này, rồi dưới nó có 'locale' (Địa Phương, ám chỉ quốc gia của người dùng) dưới nó sẽ có rất nhiều thư mục con chỉ quốc gia, với 2 ký tự, ví dụ, Việt Nam sẽ có thư mục là 'vi', rồi dưới nó là thư mục 'LC_MESSAGES'.

Nếu thư mục 'datafiles' của bạn không có thư mục 'locale' (Địa phương) và các thư mục con ở bên dưới thì các bạn phải tìm một bản cũ, có các thư mục con cho các quốc gia, và sao chép toàn bộ 'locale' ở bản cũ sang thư mục 'datafiles' của bạn, rồi sao bản 'blender.mo' lấy xuống, viết đè lên bản cũ ở 'vi/LC_MESSAGES'. Bạn Trần Ngọc Triều có phát hiện là các phiên bản thử nghiệm không cho các thư mục tiêu chuẩn như tôi nói ở đây. Các bạn phải để ý. Nhớ dùng dòng lệnh để kiểm tra xem bản mình cài nằm ở đâu và dưới nó, thư mục 'datafiles' nằm ở đâu để tìm.

Nếu các bạn sử dụng thấy có vấn đề gì, hoặc nghi hoặc, không hiểu một chữ, từ nào, muốn hỏi cho cặn kẽ, thì xin liên lạc với tôi, e-mail của tôi là [hoangduytran1960@googlemail.com](mailto:hoangduytran1960@googlemail.com), hoặc liên lạc trực tiếp bằng cách gửi thông điệp cho tôi qua tài khoản FaceBook của tôi tại [Hoang Duy Tran](https://www.facebook.com/hoangduy.tran). Cảm ơn rất nhiều. Xin đừng ngại ngùng gì, cứ liên lạc nhé.

- MacOS : 
```pwsh 
cp -f "$HOME/Downloads/blender.mo" "/Library/Application Support/Blender/2.93/datafiles/locale/vi/LC_MESSAGES/blender.mo"
```

- Linux:
```pwsh 
sudo cp -f $HOME/Downloads/blender.mo" "/usr/share/blender/2.93/datafiles/locale/vi/LC_MESSAGES/blender.mo
```

- Windows: (Cảm ơn bạn Trần Ngọc Triều trên FaceBook đã giúp tôi phần này)
```pwsh 
xcopy "%UserProfile%\Downloads\blender.mo" "C:\Program Files\Blender Foundation\Blender 2.93\2.93\datafiles\locale\vi\LC_MESSAGES\blender.mo"
