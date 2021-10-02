# Music Player

![image](https://user-images.githubusercontent.com/20525933/133104550-1e391332-4ad6-45e6-8e1c-396b1939f25d.png)


## Structure (Micro Front-end)
> - [Qiankun](https://qiankun.umijs.org/zh/guide)
> - [React / React hook](https://zh-hant.reactjs.org/)
> - [Ant Design](https://ant.design/)
> - [Spotify Web API](https://developer.spotify.com/web-api/)
> - Vanilla JS / Web-component
> - SCSS
> - Webpack / Babel
> - ESlint / Husky
> - Git sub-module

## Getting start
```
git clone https://github.com/HsienW/music-player-root.git
cd music-player-root
git submodule init
git submodule update
npm install
npm start 
```

## 說明：
#### 串接 Spotify Web API 完成的音樂播放器, 可搜尋和試聽各式音樂、歌手、專輯, 跟最新發行的專輯或單曲, 採用微前端架構目前分為 5個 sub-app。

- **Main**： 用 React 製作, 整個 qiankun 系統的啟動基座, 啟動時負責管理 Global status & Global event
- **Common** ： 用 Vanilla JS / Web-component 製作, 管理公用的 util & container, sub-app 獨立啟動時也可自行加載使用
- **Portal** ： 用 React 製作, 啟動時負責管理 User auth 與 home page 等等
- **Search** ： 用 React 製作, 啟動時負責管理 搜尋功能, 播放後導向 Collection
- **Collection** ： 用 React 製作, 啟動時負責管理播放音樂、歌手、專輯等等功能

## Demo：

- [**Demo link**](http://music-player-demo-east1.s3-website-us-east-1.amazonaws.com)
- When logging in, if you don’t have a spotify account, you can use the public demo account shown below to enter

 ![image](https://user-images.githubusercontent.com/20525933/133105455-8d892854-8ce7-43b5-b97c-f2dd1607e390.png)




