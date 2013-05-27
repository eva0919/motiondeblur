MotionDeBlur
============

DIP final project . Doing a restore for motion blur

（使用時記得修改圖片讀檔的相對路徑）
         
---
### >>> finalproject_psf <<< ###

實作PSF
解釋大概的演算法

第一個for迴圈是將圖檔讀進來
         
第二個for迴圈是建立點分散函式
這邊的位移量L是定30，可以從最上面的define去修改
而角度是45度，要改的話就要改if的y x之間關係 （ tan 三角函數 ，ex tan 45度 = 1  = y/x ） 
    
第三個for迴圈就是實作psf
PSF其實就是點分散的矩陣與原來圖檔的矩陣做convolution，就像做filter一樣
但有點不同的是，不能讓每一點相加後不處理，
所以我還多了一個變數number去做正規化的處理。
         
         
第四個迴圈將結果輸出成圖檔
         
         
