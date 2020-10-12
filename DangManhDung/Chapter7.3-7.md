Sử dụng phương thức printPrime()

![image](https://user-images.githubusercontent.com/48431650/95310542-b9d8df00-08b6-11eb-9937-b58dcf875251.png)

(a) Vẽ đồ thị luồng cho phương thức

![image](https://user-images.githubusercontent.com/48431650/95310604-ccebaf00-08b6-11eb-9544-1778b2ac783c.png)


(b) Xét ca kiểm thử *t1 = (n = 3)*, *t2 = (n = 5)*. Thiết lập một lỗi đơn giản mà t2 sẽ thường dễ tìm thấy hơn t1
* Do **n=3** trả về tất cả các số lẻ  trong khoảng 2 đến 5, còn **n=5** thì không, vậy nên một lỗi làm cho chương trình trả về số lẻ thay vì số nghuyên tố sẽ được phát hiện bởi t2 nhưng không bởi t1.
* VD: nếu kiểm thử là **if isDivisible (prime[0], curPime)**

(c) Tìm một ca kiểm thử mà đường đi kiểm thử tương ứng visit được cạnh nối điểm đầu của **while** tới **for** mà không đi qua vòng lặp while

* t = (n = 1).

(d) Liệt kê các yêu cầu kiểm thử cho bao hàm nút, cạnh, đường đi nguyên tố

* Nút: { 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14 }
* Cạnh: { (0,1) (1,2), (1,10), (2,3), (3,4), (3,7), (4,5), (4,6), (6,3),
(5,7), (7,8), (7,9), (8,9), (9,1), (10,11), (11,12), (11,14), (12,13), (13,11) }
* Đường đi nguyên tố:

        {	[0, 1, 2, 3, 4, 5, 7, 8, 9]
        	[0, 1, 2, 3, 4, 5, 7, 9]
        	[0, 1, 2, 3, 4, 6]
        	[0, 1, 2, 3, 7, 8, 9]
        	[0, 1, 2, 3, 7, 9]
        	[0, 1, 10, 11, 12, 13]
        	[0, 1, 10, 11, 14]
        	[2, 3, 4, 5, 7, 8, 9, 1, 10, 11, 14]
        	[2, 3, 4, 5, 7, 8, 9, 1, 10, 11, 12, 13]
        	[2, 3, 4, 5, 7, 9, 1, 10, 11, 14]
        	[2, 3, 4, 5, 7, 9, 1, 10, 11, 12, 13]
        	[2, 3, 7, 8, 9, 1, 10, 11, 14]
        	[2, 3, 7, 8, 9, 1, 10, 11, 12, 13]
        	[2, 3, 7, 9, 1, 10, 11, 14]
        	[2, 3, 7, 9, 1, 10, 11, 12, 13]
        	[4, 6, 3, 7, 8, 9, 1, 10, 11, 14]
        	[4, 6, 3, 7, 8, 9, 1, 10, 11, 12, 13]
        	[4, 6, 3, 7, 9, 1, 10, 11, 14]
        	[4, 6, 3, 7, 9, 1, 10, 11, 12, 13]
        	[12, 13, 11, 14]
        	[1, 2, 3, 4, 5, 7, 8, 9, 1]
        	[1, 2, 3, 4, 5, 7, 9, 1]
        	[1, 2, 3, 7, 8, 9, 1]
        	[1, 2, 3, 7, 1]
        	[3, 4, 6, 3]
        	[11, 12, 13, 11]	}


(e) Liệt kê các đường đi kiểm thử cho bao hàm nút nhưng không bao hàm cạnh
* [0, 1, 2, 3, 4, 6, 3, 4, 5, 7, 8, 9, 1, 10, 11, 12, 13, 11, 14]

(e) Liệt kê các đường đi kiểm thử cho bao hàm cạnh nhưng không bao hàm đường đi nguyên tố
* [0 1 2 3 4 6 3 7 8 9 1 2 3 4 5 7 9 1 2 3 4 6 3 4 6 3 7 8 9 1 10 11 12 13 11 12 13 11 12 13 11 14] 
