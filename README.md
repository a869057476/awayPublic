# 隐藏H5 video 在 chrome下显示下载按钮的两种方法
1.css的hack方式
video::-internal-media-controls-download-button {
    display:none;
}
video::-webkit-media-controls-enclosure {
    overflow:hidden;
}
video::-webkit-media-controls-panel {
    width: calc(100% + 30px); 
}

2.video标签中增加controlsList="nodownload"属性
