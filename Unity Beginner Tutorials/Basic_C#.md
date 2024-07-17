#Basic C#

## 1. DataType and Variables.
* DataType: là một khái niệm cơ bản để mô tả các loại giá trị mà một biến có thể lưu trữ trong bộ nhớ máy tính. Kiểu dữ liệu xác định các giá trị hợp lệ mà biến có thể chứa, cũng như các thao tác có thể thực hiện trên các giá trị đó.
* Variables: là một kiểu dữ liệu có thể thay đổi được và tên gọi tham chiếu đến một vùng nhớ nào đó trong bộ nhớ.
## 2. Constants and Enumerations.
* Enumerations(Loại liệt kê): được sử dụng để gán tên không thay đổi trong một nhóm các biến giá trị số nguyên, nó làm cho các giá trị không đổi dễ đọc hơn.
* Constants: là các giá trị bất biến được biết đến tại thời điểm biên dịch và không thay đổi trong chương trình.
  * ví dụ: ta khai báo 
    * public const int Months = 12;
    * trong ví dụ trên, hằng sô sẽ luôn là 12 và nó không thể thay đổi ngay cả chính lớp.
## 3. Operators and Expressions.
* Operators: là các ký hiệu đặc biệt thực hiện một số hoạt động trên toán hạng. Một số về toán tử như +, -, x, /, %, ++, --,...
* Expressions: là biểu thức liên quan đến các toán tử số học và được sử dụng để thực hiện các phép toán toán học.
## 4. Conditional Statements.
* If: Sử dụng câu lệnh để chỉ định một khối mã C# sẽ được thực thi nếu điều kiện là .ifTrue.
* If else: Sử dụng câu lệnh để chỉ định một khối mã sẽ được thực thi nếu điều kiện là .elseFalse.
* else if: Sử dụng câu lệnh để chỉ định điều kiện mới nếu điều kiện đầu tiên là .else ifFalse.
* Switch: Giá trị của mỗi biểu thức được so sánh với giá trị của mỗi case.
## 5. Loops (for, while, do-while, foreach)
* for: được sử dụng khi chúng ta muốn lặp mã ở số vòng nhất định.
* while: Vòng lặp lặp qua một khối mã miễn là một điều kiện được chỉ định là:whileTrue.
* do/while: vòng lặp này sẽ thực thi một lần, trước khi kiểm tra xem điều kiện có đúng hay không, thì nó sẽ lặp lại vòng lặp miễn là điều kiện đúng.
* foreach: là một vòng lặp được sử dụng để duyệt qua các phần tử của một tập hợp (collection) hoặc một mảng (array).
## 6. Break and Continue Statements
* break: sử dụng khi muốn rời khỏi vòng lặp.
  * ví dụ: vòng lặp for i < 10; i++; if i == 4 và sử dụng hàm break thì đầu ra là 1, 2, 3.
* continue: ngắt và tiếp tục vòng lặp.
## 7. Methods and Functions.
* Methods and Functions.: là một khối mã chỉ chạy khi nó được gọi, được sử dụng để thực hiện một số hành động nhất định và chúng được gọi là chức năng.
## 8. Method Definition and Invocation 
* Method Definition: là quá trình khai báo và định nghĩa một phương thức trong một lớp.
  * ví dụ:
    * public void speak(string sound){
      * console.writeLine(sound);
    * }
* Method Invocation: quá trình thực thi các câu lệnh bên trong
  * ví dụ: 
    * public static void main(){
      * Animal dog = new Animal();
      * dog.Speak("woof!")
    * }
## 9. Method Overloading.
* Method Overloading: được sử dụng khi nhiều phương thức có thể có cùng tên với khác nhau thông số
  * ví dụ:
    * int myMethod(int x)
    * float myMethod(float x)
    * double myMethod(double x, double y)
## 10. Passing Parameters (by value, by reference, out).
* By value: sử dụng khi không cần thay đổi giá trị của tham số gốc.
* by reference(ref): Sử dụng khi cần thay đổi giá trị của tham số gốc. 
* out: Sử dụng khi cần trả về nhiều giá trị từ phương thức hoặc khi biến đầu vào chưa được khởi tạo.
## 11. Return value.
* Thay đổi khai báo của hàm để cho hàm biết rằng hàm dự kiến sẽ trả về kết quả.
* Kết thúc hàm bằng từ khóa Return.
## 12. Classes and Objects.
* Mọi thứ trong C # đều được liên kết với các lớp và đối tượng, cùng với nó thuộc tính và Phương pháp. 
  * Ví dụ: trong cuộc sống thực, một chiếc xe hơi là một đối tượng. Chiếc xe có các thuộc tính, chẳng hạn như trọng lượng và màu sắc, và các phương pháp, chẳng hạn như ổ đĩa và phanh.
* Một lớp giống như một hàm tạo đối tượng.
  * ví dụ code:
  * class Car 
    {
        string color = "red";

        static void Main(string[] args)
        {
            Car myObj = new Car();
            Console.WriteLine(myObj.color);
        }
    }
## 13. Constructors and Destructors
* Constructors được gọi tự động từ thời điểm đối tượng được tạo ra. Mục đích dùng để khởi tạo dữ liệu cho dữ liệu thành viên.
* Destructors: hoạt động ngược lại với hàm Cóntructors, nó phá hủy các đối tượng của các lớp. Nó chỉ có thể được định nghĩa một lần trong mỗi lớp. Giống như các hàm Constructors, hàm Destructors được gọi tự động.
## 14. Access Modifiers (public, private, protected, internal)
* Public: có thể truy cập cho các lớp.
* Private: chỉ có thể truy cập được trong cùng một lớp.
* protected: Truy cập từ một lớp hoặc trong một lớp được thừa hưởng từ lớp đó.
* internal: có thể truy cập bất kỳ mã nào trong cùng một Assembly (thường thì là một file .exe hoặc .dll) nhưng không thể truy cập từ các Assembly khác.    
## 15. Properties (get, set)
* Setter và Getter là phương thức sử dụng để cập nhập hoặc lấy ra giá trị thuộc tính
## 16. Inheritance and Polymorphism.
* Inheritance: có 2 loại phân biệt bên trong nó gồm:
  * Quan hệ tổng quát hóa(Generation): là quan hệ được thiết lập giữa một lớp tổng quát hơn đến 1 lớp chuyên biệt (đi xuống dưới cây thừa kế). Quan hệ này dùng để phân biệt 1 loại tập hợp đối tượng thành những loại xác định hơn mà hệ thống cần làm rõ ngữ nghĩa.
  * Quan hệ chuyên biệt phân hóa hay đặc biệt hóa (Is-a): Ngược lại với quan hệ tổng quát hóa, đi lên phía trên cây thừa kế.
  * VD: Chó, mèo, cá voi đều là thuộc tính thừa kế là động vật có vú, nhưng đặc điểm của từng cá thể là khác nhau.
* Polymorphism(Tính đa hình): Cùng một cấu trúc giống nhau nhưng cho ra các kết quả khác nhau.
  * vd: ta định nghĩa 3 phương thức gồm:
    * Tau: với phương thức là public vitual với console.writeline("tau")
    * TauChien: với phương thức là public override địng nghĩa lại phương thức lớp tau console.writeline("tauchien")
    * TauDulich: với phương thức là public override địng nghĩa lại phương thức lớp tau console.writeline("tauDulich")
    * khi ta khai báo về lớp Main và khai báo 3 phương thức trên cùng một dòng lệnh là t.tenPT gọi ở hàm tau
## 17. Abstract Classes and Methods.
* Abstact classes nghĩa là chưa hoàn thiện và lớp con chỉ kế thừa Abstact class đồng thời trong Abstract class chỉ kế thừa định nghĩa của một phương thức
  * vd: public Abstract class TenPT ()
        {
          public Abstract void TenPT();
        }
* Phương thức Abstract thì phải nằm trong Abstract class, Không thể gọi Abstract class trong main vì nó mang nghĩa là chưa hoàn thiện.
  * điểm khác biệt giữa Abstract với Vitual là:
  * Abstract: bắt buộc Override.
  * Vitual: cho phép Override.
  * thứ tự của Abstract như sauL: Abstract = InComplate = Sealed = Complated. 
    * Abstract thì không thể gọi chung với với Sealed bởi vì nghĩa của Sealed là đáng dấu xong rồi.
## 18. Interface.
* Các phương thức của Interface chỉ chứa các hàm, không chứa các trường.
  * vd: Interface IAnimal
        {
          void Move();
          void Eat();
        }
## 19. Static.
* Thường được sử dụng cho các thành phần nào đó mà được dùng chung cho tất cả đối tượng khác của lớp. Hoặc nó thường được sử dụng để tạo ra các lớp gọi là (lớp tiện ích) => chứa những thành phần Support cho những lớp khác, những đối tượng khác sử dụng.
* chỉ sử dụng static cho thành phần static mà thôi.
* là thành phần không thuộc sở hữu của đối tượng mà thuộc sở hữu của lớp.
## 20. Collection and Generic.
* Collection trong C# là:
  * Các lớp hỗ trợ lưu trữ, quản lý và thao tác với các đối tượng một cách có thứ tự.
  * Các lớp này nằm trong nameSpace System.Collections
  * Các Collection thông dụng:
    * ArrayList: 
      * Là một Collections giúp lưu trữ và quản lý một danh sách các đối tượng theo kiểu mảng (truy cập các phần tử bên trong thông qua chỉ số index).
      * Rất giống Array nhưng có thể thêm hoặc xoá các phần tử một cách linh hoạt và có thể tự điều chỉnh kích cỡ một cách tự động.
    * HashTable là một Collections lưu trữ dữ liệu dưới dạng là Key - Value. Key đại diện cho khóa và kết nối tới giá trị tương đương Value
      * vd: HashTable h = new HashTable();
            h.Add("D", "dog") //"D" là Key, dog là Value.
    * SortedList: là một HashTable nhưng các giá trị được xếp theo Key, điều này giúp ta khi ta thêm mọt phần tử mới vào thì SortedList sẽ tự động sắp xếp
      * vd: SortedList sl = new SortedList();
            sl.Add(new Person("a"), 10);
    * Stack(hay còn gọi là ngăn xếp) là một cấu trúc dữ liệu hoạt động theo nguyên lý LIFO(Last In First Out). VD: khi xếp chiếc đĩa nào cuối cùng thì chiếc đĩa đó sẽ được lấy ra đầu tiên.
    * Queue(hay còn gọi là hàng đợi): là một cấu trúc dữ liệu hoạt động theo nguyên lý FIFO(First In First Out). vd: người nào đến trước thì người đó được mua vé.
  * Generic trong C# cho phép đinh nghĩa một hàm, một lớp mà không cần chỉ ra đối số kiểu dữ liệu là gì.
  * Generic cũng là một kiểu dữ liệu trong C# như int, string, bool,...nhưng nó là một kiểu tự do, tùy vào mục đích sử dụng mà nó có thể đại diện cho tất cả kiểu dữ liệu còn lại. Ngoài ra, có thể định nghĩa lớp, Interface, phương thức, delegate như kiểu generic.
## 21. Directionary.
* Về khái niệm hay cách sử dụng giống với HashTable nhưng khác về phương thức hoạt động.

  HashTable|Directionary|
  :--------|:-----------|
  Threadsafe - Hỗ trợ multi threading không đụng độ tài nguyên|Không hỗ trợ.|
  Cặp Key - Value lưu kiểu object.|Phải xác định cụ thể kiểu dữ liệu của cặp Key - value.|
  Truy xuất phần tử không tồn tại trong Hashtable sẽ không báo lỗi suy ra return null.|Truy xuất phần tử không tồn tại trong Dictionary sẽ báo lỗi|
  Hiệu quả cho dữ liệu lớn.|Không hiệu quả cho dữ liệu lớn.|
  Các phần tử được sắp xếp lại mỗi khi thêm hoặc xóa các phần tử trong Hashtable.|Các phần tử nằm theo thứ tự được thêm vào.|
  Tìm kiếm nhanh hơn.|Tìm kiếm chậm hơn.|
## 22. Array.
là một một biến lưu trữ nhiều giá trị chứ không phải là một giá trị.
vd: String[] Cars = {'a','b','c'}
## 23. List.
là tập hợp các đối tượng, truy cập bằng chỉ mục và có các phương pháp để sắp xếp, tìm kiếm và sửa đổi danh sách.
## 23. Generic and Generic Collution.
* Generic như đã giải thích ở phần mục 20, Generic giúp ta giảm thiểu việc code và tăng tính tái sử dụng. Ngoài ra, Generic còn giúp ta hạn chế truy cập nếu như không truyền đúng kiểu dữ liệu
* Collution thường giá trị bên trong đều Object, điều này gây rất nhiều khó khăn nếu như ta muốn quản lý 1 danh sách có cùng một kiểu dữ liệu. Vì Object có thể chứa mọi kiểu dữ liệu nên ta khó kiểm soát rằng việc thêm phần tử có cùng dữ liệu mà ta mong muốn hay không. Từ đó Generic Collections ra đời để giúp ta vừa có thể sử dụng được các Collections vừa có thể hạn chế lỗi xảy ra trong quá trình thực thi.
* Một số Generic Collution thông dụng:
  lớp|mô tả|
  :--|:----|
  List<T>|Là một Collections giúp lưu trữ các phần tử liên tiếp (giống mảng) nhưng có khả năng tự mở rộng kích thước. Generic Collections này là sự thay thế cho ArrayList đã học.|
  Dictionary<Tkey, TValue>|Lớp lưu trữ dữ liệu dưới dạng cặp Key – Value. Khi đó ta sẽ truy xuất các phần tử trong danh sách này thông qua Key (thay vì thông qua chỉ số phần tử như mảng bình thường). Generic Collections này là sự thay thế cho Hashtable.|
  SortedDictionary<Tkey, TValue>| Là sự kêt hợp của List và Dictionary. Tức là dữ liệu sẽ lưu dưới dạng Key – Value. Ta có thể truy xuất các phần tử trong danh sách thông qua Key hoặc thông qua chỉ số phần tử. Đặc biệt là các phần tử trong danh sách này luôn được sắp xếp theo giá trị của Key. Generic Collections này là sự thay thế cho SortedList.|
  Stack<T>|Lớp cho phép lưu trữ và thao tác dữ liệu theo cấu trúc LIFO (Last In First Out).|
  Queue<T>|Lớp cho phép lưu trữ và thao tác dữ liệu theo cấu trúc FIFO (First In First Out).| 
## 24. Delegates and Events.
* Delegate là một kiểu tham chiếu, tham chiếu tới một hàm hoặc một phương thức. Có thể thay đổi RunTime.
* Lưu ý: 
  * khi muốn một hàm tham chiếu tới delegate thì phải thỏa mãn điều kiện là tham số thứ nhất có kiểu dữ  liệu dữ liệu trả về và tham số thứ hai là tham số đầu vào.
  * Không khai báo trong hàm mà khai báo ngoài hàm.
* Mục đích của delegate là khi tạo một biến và muốn biến đó tham chiếu tới hàm thông qua delegate.
* Cách viết và sử dụng Delegate như sau:
* Code: delegate int MyDel (string S);
        static void main(){
          MyDel md = new MyDel(TenPT1);
          MyDel md = new MyDel(TenPT2);
          MyDel multicast = TenPT1 + TenPT2;

          multicast += (numberSTR);
          // vd khi ta muốn loại bỏ TenPT2
          multicast -= TenPT2
        }

        static int TenPT1(string Value){

        }

        static int TenPT2(string Value){

        }
* ví dụ về code theo phương thức Call-Back Function
  delegate int MyDele(String S);
  Static void main(){
    MyDele ten = new MyDele(showString);

    Name(showString);
  }

  static void Name(MyDele showName){
    string name = Console.readLine();
    showName(name);
  }

  Static void int showString( String show){
    Console.writeLine(show);
  }
* Event với Delegate.
* cú pháp để thực hiện Event: public event TenDelegate TenEvent;
* Event là delegate với mục đích để cho lớp khác hoặc đối tượng cha của đối tượng hiện tại ủy thác (Định nghĩa) hàm vào trong đó.
* Event với Delegate nhưng thỏa mãn 2 điều kiện:
  * Delegate là kiểu trả là void
  * Delegate có 2 tham số, tham số thứ nhất có kiểu dữ liệu là Object, tham số thứ hai có kiểu EventArgs.Object chính là đối tượng phát sinh, sự kiện, EventArgs chính là class giữ thông tin mà đối tượng gửi kèm trong quá trình phát sinh sự kiện.
  => lúc này, thay vì chúng ta dùng delegate do chúng ta tự tạo thì .Net có sẵn delegate tên là EventHander theo chuẩn.
  ví dụ code về Event:
  delegate void Tendele (string name);
  class main{
    static void main()
    {
      ....
    }
  }
  public class{
    public event Tendele Tenevent;
    private string _name;
    public string name{
      set {
        return _name;
      }
      get {
        _name = value;
      }
    }
  }
## 25.   
        
  