# Illustrator 專案

> 紀錄一些Illustrator筆記及作品。

## 資料夾結構
```
+--- Illustrator                    專案資料夾
    +--- Note                           筆記
    +--- Record                         作品
    +--- Templet                        範本檔案
        +--- ClothinAndAccessories          服飾、配件
        +--- Print                          列印用
    +--- Tracing                        描圖
    +--- Readme.md                      說明文件
```

## `Git LFS`教學
> 過大的檔案要用Git LFS，常用於設計檔案，二進制檔案。

1. 安裝 Git-lfs
    * Windows
        > 到[Git-lfs官網](https://git-lfs.github.com/) 下載安裝包並安裝。
2. 加入追蹤設定`.gitattributes`
   > 選擇您希望 Git LFS 管理的文件類型，或直接編輯 .gitattributes。
   > 此專案主要追蹤 illustrator檔案`*.ai`
   * 初始化
        ``` bash
        git init
        ```
   * 以`git lfs`追蹤`*.ai`，此動作將生成`.gitattributes`
        ``` bash
        git lfs track "*.ai"
        ```
   * 追蹤設定加入
        ``` bash
        git add .
        ```
   * 推至儲存庫
        ``` bash
        git remote add origin https://github.com/orange9982239/illustrator.git
        git branch -M main
        git push -u origin main
        ```

## 亂流
> Hyperv 虛擬交話機在wifi下分享網路，會變成bridge模式，影響Git LFS上傳檔案。
![暫時關掉分享網路給VM](https://raw.githubusercontent.com/orange9982239/ImageHosting/master/images/20220424205639.png)

## 參考
   * https://git-lfs.github.com/