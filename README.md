Câu 1. Phân biệt Value Types và Reference Types trong C# về cách lưu trữ bộ nhớ Stack và Heap
-Value Types (kiểu giá trị) là kiểu dữ liệu mà biến lưu trữ trực tiếp giá trị của nó. Các kiểu dữ liệu thuộc nhóm này gồm số nguyên, số thực, kiểu logic, ký tự và cấu trúc.Value Type lưu trực tiếp giá trị.Value Type có thể nằm trên Stack hoặc trong đối tượng trên Heap.Về bộ nhớ, Value Type có thể được lưu trên Stack khi là biến cục bộ hoặc có thể nằm trong vùng nhớ của một đối tượng trên Heap, tùy vào ngữ cảnh sử dụng.
-Reference Types (kiểu tham chiếu) là kiểu dữ liệu mà biến lưu trữ một tham chiếu đến đối tượng thay vì lưu trực tiếp toàn bộ đối tượng. Các đối tượng của Reference Type thường được cấp phát trên Heap.Reference Type lưu tham chiếu đến đối tượng.Đối tượng của Reference Type thường được lưu trên Heap.

Câu 2. Phân biệt Init-only Properties (init) trong C# 9/10 với set thông thường và nêu trường hợp sử dụng thực tế
-set thông thường cho phép thuộc tính được gán giá trị khi khởi tạo đối tượng và tiếp tục được thay đổi sau khi đối tượng đã được tạo.set cho phép thay đổi giá trị thuộc tính sau khi tạo đối tượng.set phù hợp với những thuộc tính có thể cần cập nhật trong quá trình chương trình hoạt động.
-init là thuộc tính được giới thiệu trong C# 9, cho phép thiết lập giá trị trong quá trình khởi tạo đối tượng nhưng không cho phép thay đổi giá trị đó sau khi đối tượng đã được khởi tạo.init chỉ cho phép thiết lập giá trị trong quá trình khởi tạo.init phù hợp với những thuộc tính cần được thiết lập một lần và không nên thay đổi sau đó.
Trường hợp thực tế là khi tạo sinh viên, MaSV được thiết lập một lần lúc khởi tạo. Sau đó MaSV không thể thay đổi, trong khi HoTen có thể thay đổi.

Câu 3. Phân biệt virtual trong lớp cha và override trong lớp con trong cơ chế đa hình
-virtual được sử dụng trong lớp cha để khai báo một phương thức có thể được lớp con thay đổi cách thực hiện.virtual được khai báo ở lớp cha.virtual cho phép phương thức được ghi đè.
-override được sử dụng trong lớp con để ghi đè phương thức đã được khai báo virtual hoặc abstract ở lớp cha.override được khai báo ở lớp con.override thực hiện việc ghi đè phương thức.
-Trong cơ chế đa hình (Polymorphism), khi một đối tượng của lớp con được tham chiếu thông qua kiểu của lớp cha, chương trình có thể gọi phiên bản phương thức được ghi đè của lớp con.

Câu 4. Tại sao thành viên static của lớp không thể được truy cập thông qua một đối tượng được tạo bằng new?
Thành viên static thuộc về lớp (class) chứ không thuộc về một đối tượng cụ thể.
Khi một thành viên được khai báo là static, thành viên đó được dùng chung cho toàn bộ lớp và không tạo ra một bản sao riêng cho mỗi đối tượng.
Vì vậy, thành viên static được truy cập thông qua tên lớp thay vì thông qua một đối tượng được tạo bằng new.
