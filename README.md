# blender_ui - Giao Diện Người Dùng của Blender trong Tiếng Việt
Đây là đề án phiên dịch giao diện phần mềm nguồn mở 
[Blender](https://www.blender.org/download/) sang tiếng Việt. 
Các bạn có thể lấy bản 
[blender.mo](https://github.com/hoangduytran/blender_ui/blob/main/3x/blender.mo) này về máy và nạp vào thư mục tương ứng (xem dưới đây) để có thể đổi giao diện phần mềm sang tiếng Việt và sử dụng nó trong ngôn ngữ mẹ đẻ của mình. 
Đương nhiên, bản này hiện cũng đang trên đà được tiến hành, và hằng ngày sẽ có bản cập nhật các thay đổi mới nhất.
Mong các bạn để ý ngày và giờ xuất xưởng mà tôi đăng lên đây để xem và lấy bản mới nhất về máy.

Sau khi lấy xuống máy thì đưa vào thư mục của phần mềm trên máy bằng cách mở một cửa sổ dòng lệnh và đánh dòng lệnh ví dụ sau đây, tùy theo hệ điều hành mà bạn sử dụng:

Tôi sử dụng phiên bản 2.93 trong các ví dụ dưới đây. Nếu bạn sử dụng 3.0 hoặc 3.1 chẳng hạn, thì thay giá trị 2.93 bằng 3.0 hoặc 3.1 nhé.

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
