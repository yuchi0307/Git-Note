# Git-Note
關於我常忘記的 git 指令紀錄
<h2>React 上傳至 gh-pages </h2></br>
<div>
<ol>
  <li>terminal 確認所在位置為: master branch</li>
  <li>%npm run build (專案出現 build 資料夾)</li>
  <li>打開專案的 package.json 加入"homepage: https://yuchi0307.github.io/repo名稱",</li>
  <li>%npm install --save gh-pages</li>
  <li>在 package.json 的"scripts": 加入</br>
  "predeploy": "npm run build",</br>
  "deploy": "gh-pages -d build",</br>
  </li>
  <li>%npm run deploy</li>
  <li>回到 github 檢查 branch 是否成功新增 gh-pages branch</li>
</ol>
</div>
<section>
  <h2>上傳後若有更新code</h2></br>
  <ol>
  <li>%git push origin:gh-pages</li>
  <li>git init</li>
  <li>npm install --save gh-pages</li>
  <li>npm run deploy</li>
  </ol>
</section>
