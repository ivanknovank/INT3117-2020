Cho 4 đồ thị sau

![image](https://user-images.githubusercontent.com/48431650/94986617-55521300-058a-11eb-9dc4-d679500cbb4d.png)

(a) Vẽ đồ thị
* Graph I

![image](https://user-images.githubusercontent.com/48431650/94986488-6d756280-0589-11eb-9b61-065c11d4bf04.png)

* Graph II

![image](https://user-images.githubusercontent.com/48431650/94986530-bf1ded00-0589-11eb-8496-c64efead7e32.png)

* Graph III

![image](https://user-images.githubusercontent.com/48431650/94986576-2045c080-058a-11eb-93e7-f926c2ba6290.png)

* Graph IV

![image](https://user-images.githubusercontent.com/48431650/94986661-a7933400-058a-11eb-8434-5f082a25932b.png)


(b) Liệt kê tất cả các du-path liên quan đến x

* Graph I:

        i	[1,2,8]
        ii	[1,2,3,5,6]
        iii	[4,3,5,6]
        iv	[4,3,5,7,2,8]
        v	[4,3,5,6,7,2,8]

* Graph II:

        i	[1,2,3]
        ii	[1,2,6]
        iii	[3,4,5,2,3]
        iv	[3,5,2,3]
        v	[3,4,5,2,6]
        vi	[3,5,2,6]

* Graph III:

        i	[1,2,3]
        ii	[1,2,3,5]
        iii	[1,2,6]
        iv	[4,5,2,3]
        v	[4,5]
        vi	[4,5,2,6]

* Graph IV:

        i	[1,2,3,5]
        ii	[1,2,3,4,5]
        iii	[1,2,6]
        iv	[5,2,3,5]
        v	[5,2,3,4,5]
        vi	[5,2,6]

(c) Xác định du-path nào mà các đường đi kiểm thử tour được.

* Graph I

Test | Tour | Side-trip
-|----- | -----
t1|i| 
t2| |i
t3|ii|i
t4|iv| 
t5|iii, v| 
t6| |iii, iv, v

* Graph II

Test | Tour | Side-trip
-|----- | -----
t1|ii| 
t2|i,iii,vi|ii,iv,v,vi 
t3|i,iv,v|ii,iii,vi
t4|i,vi|ii,iv 

* Graph III

Test | Tour | Side-trip
-|----- | -----
t1|i, ii|iii
t2|i, iv,vi| 

* Graph IV

Test | Tour | Side-trip
-|----- | -----
t1|iii|
t2|ii,vi|i,iii,iv,v 
t3|i,v,vi|ii,iii,iv


(d) Liệt kê một bộ kiểm thử tối giản thỏa mãn bao hàm toàn defs liên quan tới x.

* Graph I
 
        {t1,t4} hoặc {t1,t5} hoặc {t3,t4} hoặc {t3,t5}

* Graph II

        {t2} hoặc {t3} hoặc {t4}

* Graph III

        {t2}


(e) Liệt kê một bộ kiểm thử tối giản thỏa mãn bao hàm toàn uses liên quan tới x.

* Graph I

        {t1,t3,t5}

* Graph II

        {t1,t3} hoặc {t1,t2}

* Graph III

        {t1,t2,[1,2,6],[1,2,3,4,5,2,3,5,2,6]}


(f) Liệt kê một bộ kiểm thử tối giản thỏa mãn bao hàm toàn du-path liên quan tới x.

* Graph I

        {t1,t3,t4,t5}

* Graph II

        {t1,t2,t3}

* Graph III

        {t1,t2,[1,2,6],[1,2,3,4,5,2,3,5,2,6]}

