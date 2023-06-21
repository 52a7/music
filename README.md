一个简易的音乐播放器的代码示例，使用 Python 和 Pygame 库实现：


import pygame

# 初始化Pygame
pygame.init()

# 创建音乐播放器
pygame.mixer.init()

# 音乐文件路径
music_file = "path/to/music_file.mp3"

# 加载音乐文件
pygame.mixer.music.load(music_file)

# 播放音乐
pygame.mixer.music.play()

# 等待音乐播放完成
while pygame.mixer.music.get_busy():
    continue

# 停止音乐播放
pygame.mixer.music.stop()

# 退出Pygame
pygame.quit()



请确保将 "path/to/music_file.mp3" 替换为你实际的音乐文件的路径。这段代码使用 Pygame 的 mixer 模块来实现音乐的播放和停止。它会加载音乐文件并开始播放，然后等待音乐播放完成后停止播放，并最后退出 Pygame。

请注意，你需要确保已安装 Pygame 库，并且音乐文件的路径是正确的。另外，支持的音频文件格式取决于你的系统和 Pygame 的配置。
