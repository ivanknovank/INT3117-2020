Cho phương thức **search()**:

![image](https://user-images.githubusercontent.com/48431650/94504990-51de2500-0234-11eb-9b3b-b42ed8c8da72.png)

và sự phân vùng các đặc trưng sau:

![image](https://user-images.githubusercontent.com/48431650/94505017-602c4100-0234-11eb-8d1e-15535ad5b567.png)


(a) "Location of element in list" không đúng ở tính rời rạc. Lấy ví dụ để minh họa.

    VD:*list = [3, 4, 3]; e = 3* hay *list = [3]; e = 3*.
    "Location of element in list" không dự đoán trước được là vị trí của phần tử có thể ở cả đầu và cuối danh sách.

(b) "Location of element in list" không đúng ở tính đầy đủ. Lấy ví dụ để minh họa.

    VD:*list = [5, 3]; e = 4*.
    "Location of element in list" không có ô dành cho phần tử không nằm trong danh sách.

(c) Hãy tạo một hoặc nhiều phân vùng mới phù hợp với mục đích của "Location of element in list" nhưng không bị sai ở tính đầy đủ và tính rời rạc.

    Charateristic: Whether e is first in the list
        Block 1: true
        Block 2: false
    Charateristic: Whether e is last in the list
        Block 1: true
        Block 2: false
