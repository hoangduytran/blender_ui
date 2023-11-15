# blender_ui - Giao Diện Người Dùng của Blender trong Tiếng Việt
Đây là đề án phiên dịch giao diện phần mềm nguồn mở 
[Blender](https://www.blender.org/download/) sang tiếng Việt. 

Bấm vào đường dẫn để lấy bản tương ứng với phiên bản 'blender.mo' mình cần
- 2.79b [blender.mo](https://github.com/hoangduytran/blender_ui/blob/main/2.79b/blender.mo)
- 2.83.9 [blender.mo](https://github.com/hoangduytran/blender_ui/blob/main/2.83/blender.mo)
- 3.x [blender.mo](https://github.com/hoangduytran/blender_ui/blob/main/3x/blender.mo)

Sau khi đã tải các bản 'blender.mo' trên về máy và nạp vào thư mục tương ứng (xem dưới đây) để có thể đổi giao diện phần mềm sang tiếng Việt và sử dụng nó trong ngôn ngữ mẹ đẻ của mình. 

Sau khi lấy xuống máy thì đưa vào thư mục của phần mềm trên máy bằng cách mở một cửa sổ dòng lệnh và đánh dòng lệnh ví dụ sau đây, tùy theo hệ điều hành mà bạn sử dụng.

Tôi sử dụng phiên bản 2.93 trong các ví dụ dưới đây. Nếu bạn sử dụng 2.79b, 3.0 hoặc 3.1 chẳng hạn, thì thay giá trị 2.93 bằng 3.0 hoặc 3.1 nhé. Đường dẫn cơ bản là từ thư mục 
```pwsh
datafiles 
```
Các bạn phải có thư mục này, rồi dưới nó có 
```pwsh
locale 
```
(Địa Phương, ám chỉ quốc gia của người dùng) dưới nó sẽ có rất nhiều thư mục con chỉ quốc gia, với 2 ký tự, ví dụ, Việt Nam sẽ có thư mục là 
```pwsh
vi 
```
rồi dưới nó là thư mục 
```pwsh
LC_MESSAGES
```
Nếu thư mục 
```pwsh
datafiles 
```
của bạn không có thư mục 
```pwsh
locale 
```
(Địa phương) và các thư mục con ở bên dưới thì các bạn phải tìm một bản cũ, có các thư mục con cho các quốc gia, và sao chép toàn bộ 
```pwsh
locale 
```
ở bản cũ sang thư mục 
```pwsh
datafiles 
```
của bạn, rồi sao bản **blender.mo** lấy xuống, viết đè lên bản cũ ở thư mục
```pwsh
vi/LC_MESSAGES
```
Bạn Trần Ngọc Triều có phát hiện là các phiên bản thử nghiệm không cho các thư mục tiêu chuẩn như tôi nói ở đây. Các bạn phải để ý. Nhớ dùng dòng lệnh để kiểm tra xem bản mình cài nằm ở đâu và dưới nó, thư mục 'datafiles' nằm ở đâu để tìm.

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
```

## Một điều nhắc nhỏ:

Như nói đến trong phần này của bản [Hướng Dẫn Sử Dụng](https://docs.blender.org/manual/en/3.1/advanced/blender_directory_layout.html), Blender để các cấu hình của mình ở hai nơi, thư mục cài bản nhị phân thi hành (blender.exe, hoặc blender), hay SYSTEM (Hệ Thống), và tại địa chỉ thư mục NHÀ ($HOME, %USERPROFILE%). Thư mục $HOME, nếu tồn tại, thì sẽ được cập nhật và sử dụng trước (có quyền ưu tiên hơn cả).

Nếu các bạn đưa bản 'blender.mo' vào thư mục NHÀ một cách miễn cưỡng, và khi bật lên, không thấy mục ngôn ngữ trong cấu hình giao diện không có gì thì có nghĩa là nó thiếu các văn bản và thư mục cần có về ngôn ngữ. Nếu thế, thì các bạn lần vào thư mục cài đặt bản nhị phân thi hành (executable binary), tức là bản (blender.exe, hoặc blender) và tìm thư mục 

```pwsh
locale
```

ở dưới

```pwsh
datafiles
```

và sao chép toàn bộ thư mục 

```pwsh
locale
```

về thư mục tại ($HOME, %USERPROFILE%) của mình.

Chẳng hạn, đối với phiên bản 2.83.9, trên máy MacBook Pro (hệ điều hành OSX) thì tôi phải sao từ

```pwsh
/Applications/Blender 2.83.9.app/Contents/Resources/2.83/datafiles/locale
```

sang

```pwsh
/Users/hoangduytran/Library/Application Support/Blender/2.83/datafiles
```

Dòng lệnh tôi sẽ phải sử dụng trên cửa sổ bàn giao tiếp đánh dòng lệnh là:

- tạo thư mục ở địa chỉ NHÀ
- sao chép toàn bộ thư mục 'locale' ở nơi cài đặt Blender, sang địa chỉ NHÀ

```pwsh
mkdir -p "/Users/hoangduytran/Library/Application Support/Blender/2.83/datafiles"
cp -a "/Applications/Blender 2.83.9.app/Contents/Resources/2.83/datafiles/locale" "/Users/hoangduytran/Library/Application Support/Blender/2.83/datafiles"
```

Sau khi làm xong việc trên thì mình có thể đưa bản [blender.mo](https://github.com/hoangduytran/blender_ui/blob/main/2.83/blender.mo) tải về máy vào thư mục nhà của tôi tức thư mục:

```pwsh
"/Users/hoangduytran/Library/Application Support/Blender/2.83/datafiles/locale/vi/LC_MESSAGES"
```

và từ giờ trở đi, Blender sẽ vào thư mục nhà trên của tôi để lấy các bản ngôn ngữ ở đó, bỏ qua hẳn thư mục cài đặt:

```pwsh
"/Applications/Blender 2.83.9.app/Contents/Resources/2.83/datafiles/locale"
```