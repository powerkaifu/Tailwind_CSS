# Tailwind CSS

Tailwind CSS 屬於實用工具類型（Utility）的 CSS 框架，與 Bootstrap 最大的不同點在於 Tailwind CSS 全力支持使用工具類型的 Class 讓設計者完成客製化的版型，甚至可以不用寫 CSS 或鮮少就能完成版型設計。

它可在 HTML 文件的元素內靈活操作 Class，也因為這特性，必須使用 Class 去組合各種 CSS 的觀念技巧，類似一種組合技的概念，所以客製化切版速度非常快，但比起 Bootstrap，它更考驗了設計者對於 CSS 的了解以及 Tailwind CSS 的環境設定。

[Tailwind CSS 大全](https://powerkaifu.github.io/2020/09/24/lesson-tailwind-css/)

## 實驗場

### [兩欄](https://powerkaifu.github.io/Tailwind_CSS/src/2020-09-26-two-column.html)

- 2020/09/26 - inline-block 與 float 排版 測試

  inline-block 沒有 font-size:0 class，需自訂義。

### [三欄](https://powerkaifu.github.io/Tailwind_CSS/src/2020-09-26-three-column.html)

- 2020/09/26 - inline-block 與 float 排版 練習

  三欄練習。

### [骰子](https://powerkaifu.github.io/Tailwind_CSS/src/2020-09-26-dice.html)

- 2020/09/26 - Position 測試

  測試 Tailwind 對於定位的支援，其定位位置適合大方向，細節較不足，因此自訂了 10% 到 90% 的 Class，盒陰影部分難達成想要的效果，或許應該朝自訂義方向去解決？但是想睡搞搞了．．．

### [彈性盒](https://powerkaifu.github.io/Tailwind_CSS/src/2020-09-29-flexbox.html)

- 2020/09/26 - Flex box 測試

  彈性盒測試。

### [切版](https://powerkaifu.github.io/Tailwind_CSS/src/2020-09-29-layout.html)

- 2020/09/26 - 切版問題集

  - 高度：預設只有支援到 h-64（16rem = 256px），需自訂增加，增加了 h-72、h-88、h-500(500px)、h-600(600px)。
  - 背景：可以設定漸層，但沒有設定 url 背景圖，需在設定檔自訂 url 背景圖。
  - 文字陰影：沒有文字陰影的 Class，可以在 tailwind.css 新增以下。

    ```css
    @responsive {
      .text-shadow {
        text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.5);
      }
    }
    ```
