###ASCII字符集

每个字符由一个唯一的7位整数表示，使用每个字节的低7位。

###Unicode

* 有三种编码形式，允许数据以字节、字、双字格式存储。

####UTF-8：

* ASCII码在UTF-8中占用一个字节，其字节与ascII值是一样的。
* <font color=red>是互联网领域的通用编码.</font>
* 变长编码使用1~4个字节表示一个Unicode序号的字，根据不同的字而变化字节长度。
  `对于单字节的符号，首位为0，后面7位是其unicode序号。因此对于英语字母，UTF-8编码和ASCII码是相同的。`
  `对于n(2-4)字节的符号，第一个字节的前n位都设为1，第n+1位设为0，后面字节的前两位一律设为10。剩下的没有提及的二进制位，全部为这个符号的unicode码。`


####UTF-16：

* 用于访问效率和存储空间并存的环境中。每个字符用16个二进制数据位编码。
* <font color=red>是windows内核编码.</font>

####UTF-32：

* 用于不太关心存储空间的环境中，每个字符都使用32个二进制数据位编码，宽度固定。
* 把长度较小的unicode值复制到长度较大的unicode值中不会丢失任何数据。

###ASCII字符串：

* 一个或多个字符的序列称为字符串。即是存储内存中包含ascii的连续字节。（空字符结尾的字符串是以包含0的字节结尾的字符串。

###ASCII码控制字符：

字符值范围在0-31之间
