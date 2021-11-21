# blender_ui
Đây là đề án phiên dịch giao diện phần mềm nguồn mở 
[Blender](https://www.blender.org/download/) sang tiếng Việt. 
Các bạn có thể lấy bản 
[blender.mo](blender_ui/tree/main/3x/blender.mo) này về máy và nạp vào thư mục tương ứng (xem dưới đây) để có thể đổi giao diện phần mềm sang tiếng Việt và sử dụng nó trong ngôn ngữ mẹ đẻ của mình. 
Đương nhiên, bản này hiện cũng đang trên đà được tiến hành, và hằng ngày sẽ có bản cập nhật các thay đổi mới nhất.
Mong các bạn để ý ngày và giờ xuất xưởng mà tôi đăng lên đây để xem và lấy bản mới nhất về máy.

Sau khi lấy xuống máy thì đưa vào thư mục của phần mềm trên máy bằng cách mở một cửa sổ dòng lệnh và đánh dòng lệnh ví dụ sau đây, tùy theo hệ điều hành mà bạn sử dụng:

Tôi sử dụng phiên bản 3.0 trong các ví dụ dưới đây. Nếu bạn sử dụng 2.93 chẳng hạn, thì thay giá trị 3.0 bằng 2.93 nhé.

- MacOS : 
```pwsh 
cp -f $HOME/Downloads/blender.mo 
/Users/$USER/Library/Application Support/Blender/3.0/datafiles/locale/vi/LC_MESSAGES/blender.mo
```

- Linux:
```pwsh 
cp -f $HOME/Downloads/blender.mo 
$HOME/.config/blender/3.0/datafiles/locale/vi/LC_MESSAGES/blender.mo
```

- Windows:
```pwsh 
xcopy "%UserProfile%\Downloads\blender.mo 
%USERPROFILE%\AppData\Roaming\Blender Foundation\Blender\3.0\datafiles\locale\vi\LC_MESSAGES\blender.mo"
