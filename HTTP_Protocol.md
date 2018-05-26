
# HTTPЭ��
ȫ��:Hypertext Transfer Protocol(���ı�ת��Э��)

**HTTP��һ����״̬��Э��**��ÿһ�����󲻻ᱣ��ͻ��˺ͷ���˵�״̬

## 1. ����HTTP�Ľ�������
����ͼ����
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP1.png)

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP2.png)

�ʣ�httpЭ����ʲô�ط��������ã�

����tcp/ipЭ������ϣ�������httpЭ��

�ʣ�httpЭ����ͨ���е�������ʲô��

��message(��Ϣ)

�ʣ�������ʲô��

�𣺷���һ��http��request message

## 2. ����Ӧ�ò�Э��
�ȿ�һ��OSIģ�ͺ�TCP/IPģ��

����ͼƬ����

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_OSI.png)

---

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_TCP_IP.png)

**���ص�1����HTTPЭ������Ӧ�ò�Э��**

**���ص�2����tcp�Ǵ���㣬���ݱ��ĵĴ��䣬�������ݵĸ�ʽ�����������ݱ��ġ�**

## 3.����CS�ܹ�

Client�ˣ���HTTP Agent�Ĺ����������(Browser)ʵ�֣��ֳ�BS�ܹ�

HTTP Server�ˣ����ṩ���ı�(�ѷ�չΪ��ý��)����

��ý�壺����Link������ͼƬ��Ƶ��

����һ��Ӧ:ֻ����Client������������Server�ٷ�����Ӧ

## 4. ��״̬��Cookie & Session
**���ص�3����Ϊ��ʹhttp��״̬��ʹ��Cookie��Session**

## 5. �����ı�
HTTPЭ����Ӧ�ò��ǻ����ı���

## 6. �־�����
ʲô�ǳ־����ӣ�����"�־�"�����ӡ�

**���ص�4�������䱨���ǿ�����TCP����**

Ϊ�����һ��HTTP����**�������Ϳͻ���֮��Ҫ����һ��TCP���������䱨��**�������������Ժ�һ�㶼��ֱ�Ӱ����رգ�����������ģʽ����������**���������ʹ��Ч�ʵĽ���**��ԭ�����£���

1��ÿ�ν������ӵ�ʱ��Ҫ�����������ֵȱ���ĳ������ӵ��һ������һֱʹ�õ����ӣ�Ҳ����ζ��ֻ��Ҫ����һ�����ӵĽ��������ʡȥ��ÿ�ν������ӵ�ʱ�䡣

2��ʹ�ù������ӻ���½����������ٶȻ��һЩ��������Ϊ**TCP����������**�����ԣ�ÿ�ν����µ����ӣ������Ѿ������õĵ������ٶȿ졣

����ͼƬ����

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_chijiulianjie1.png)

---

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_chijiulianjie2.png)


**���ص�5����tcp���Ӹ���**������һ����Ӧһ�Σ�Ȼ��������һ����Ӧһ�Σ�������ر�tcp���ӡ�����ͼ��

�ʣ���ν����־����ӣ�
��ʹ��**keep-alive**

�ͻ����ȷ���������connection��keep-alive����ʽ�����������������������ܵ�����Ļ���Ӧ�оͻ����connection��keep- alive.����ʹ��keep-alive�ײ�����һЩ���ڳ־����ӵĲ�����**timeout��ʾ����ʱ�䣬max��ʾϣ�����������־������ϴ�����ٸ�HTTP����**��������Щ������**��ŵֵ��Ҳ����˵��ʱ�����Է���**��

ע��㣺���Ҫ���ó־����ӣ���ô��һ��Ҫ����ȷ��content-length����������峤�ȵ��ײ�����Ϊ�־����ӻ������Ĵ���HTTP���񣬶��ж�������HTTP�� ��֮��ķֽ����ǿ�content-length���ߵ�����ĳ����ˣ���������û�и�������ĳ��ȵĻ�����ô��û�취֪�������������������ˡ�


## 7. ���߻� pipelining
����**��ˮ�߼���**

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_pipelining.png)

**���ص�6����pipelining**���Ѷ��HTTP����ŵ�һ��TCP������һһ���ͣ����ڷ��͹����пͻ��˲���Ҫ�ȴ���������ǰһ���������Ӧ��

**���ص�7������ͷ����**�������Ҫ����˳�����������ǰһ������ǳ���ʱ����ô�������󶼻��ܵ�Ӱ�졣�ͻ���Ҫ���շ��������˳����������Ӧ��

**���ص�8����**����ڵ����ڵĵڶ���ͼ�����߻��Ľ�֮�����ǲ���Ҫ�ȴ�����˶���һ������������Ӧ֮��ſ��Է�����һ������

## 8. URL
��λҪ����ͨ�ŵķ��������Լ���Ҫ��ȡ����Դ

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_url.png)

## 9. HTTP_Method
**���ص�9����ָʾServer���������ԴӦ��������Ϊ/����**

* GET:�����ֻ����������Դ���ظ��ͻ��ˣ���Ӧ�����������á�

* POST:�ͻ��˽��½���Դ���������Я���������У�ʹ����˴���һ������Դ��

* PUT:�ͻ����ṩ��������Դ��Ϣ������ˣ�����˾ݴ˸��¼�����Դ�򴴽�����Դ��

* DELETE:�����ɾ��ָ������Դ��

* PATCH:�ͻ����ṩָ����Դ�Ĳ�����Ϣ������˾ݴ˶Լ�����Դ���ֲ����¡�

* HEAD:����˹�����GET����һģһ������Ӧͷ�����ظ��ͻ��ˣ����ڿͻ��˻�ȡ����Դ��Ԫ��Ϣ���������崫�䡣�����ڼ����Դ�Ƿ��ѸĶ���

* TRACE���ؿͻ�����������ЩԾ�㵽���˷���ˣ��м������������ת��������ʱӦ���Լ���IP��DNS�������ӵ�ͷ����Via�ֶ��С���������ϡ�

* OPTIONS:����˷��ظ�URL֧�ֵĶ���P������ͨ������*�������Ǿ�����Դ��

**���ص�10����GET��HEAD���������ĸ�WEB SERVER ����ʵ��GET��HEAD��ʵ��������������֮�󣬲��ܳ�ΪHTTP SERVER�����ܸ������ṩ��Դ**

![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_Method.png)

HTTP Server����֧��GET��HEAD����������������ѡ��Ҳ�����Զ��������չ��

## 10. ״̬��
* 1XX����Ϣ�������ѱ�������յ�����������ն���P/1.1��֧��

* 2XX���ɹ��������ѳɹ���������յ������Ⲣ�������

* 3XX���ض�����Ҫ��һ���Ĳ���������ɴ�����

* 4XX���ͻ��˴��������дʷ���������޷���ִ��

* 5XX������˴��󣬷�����ڴ�������Ĺ����з�������

---
**���ص�11�����ھŽں͵�ʮ��С�᣺��**

URL+HTTP Method��ʵ��Client����Server����δ������󡣱�����Server�����ݵ���ɾ�Ĳ�

Status Codes��ʵ��Server����Client����ν�����Ӧ��������ʾ��ȷҳ�������ת����һ��urlȥ��

---

## 11. ��Ϣ��ʽ
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_MessageFormat.png)

<>�������Ǳ�ѡ

**RequestMessage**
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_RequestMessage.png)


**ResponseMessage**
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_ResponseMessage.png)

## 12.HTTPͷ��

### **HTTPͷ���ֶνṹ**

ͷ���ֶεĽṹΪkey-vlaue�Ľṹ��

> ͷ���ֶ��� : �ֶ�ֵ 
> ���� Content-Length: 139

�ֶ�ֵ��Ӧ����ͷ���ֶ��������ж��ֵ

> ͷ���ֶ��� : �ֶ�ֵ1,�ֶ�ֵ2 �� 
> ���� Keep-Alive: timeout=15,max=100


### ͨ��ͷ���ֶ�

**�����ĺ���Ӧ���Ķ��õ����ֶΡ�**

ͷ���ֶ��� | ˵��
- | :-: 
Cache-Control | ���ƻ������Ϊ 
Connection    | �����ײ������ӵĹ��� 
Date | �������ĵ�����ʱ�� 
Pragma | ����ָ�� 
Trailer | ����ĩ�˵�ͷ��һ�� 
Transfer-Encoding | �ƶ���������Ĵ�����뷽ʽ 
Upgrade | ����Ϊ����Э�� 
Via | ���������������Ϣ 
Warning | ����֪ͨ 

### ʵ��ͷ���ֶ�

**����������Ӧ���ĵ�ͷ���ֶΣ���������Դ����ʱ���Լ�ʵ����й���Ϣ**

ͷ���ֶ��� | ˵��
- | :-: 
ͷ���ֶ��� | ˵�� 
Allow | ��Դ��֧�ֵ�HTTP���� 
Content-Encoding | ʵ���������õı��뷽ʽ 
Content-Language | ʵ���������Ȼ���� 
Content-Length | ʵ������Ĵ�С����λ���ֽڣ� 
Content-Location | �����Ӧ��Դ��URI 
Content-MD5 | ʵ������ı���ժҪ 
Content-Range | ʵ�������λ�÷�Χ 
Content-Type | ʵ�������ý������ 
Expries | ʵ��������ڵ�����ʱ�� 
Last-Modified | ��Դ������޸����� 

### ����ͷ���ֶ�

������ʹ�õ�ͷ���ֶΣ�����������ĸ������ݡ��ͻ���Ϣ����Ӧ���ȼ�����Ϣ��


ͷ���ֶ��� | ˵��
- | :-: 
Accept | �û������ɴ�����ý������ 
Accept-Charset | ���ȵ��ַ��� 
Accept-Encoding | ���ȵ����ݱ��� 
Accept-Language | ���ȵ����ԣ���Ȼ���ԣ� 
Authorization | Web��֤��Ϣ 
Expect | �ڴ����������ض���Ϊ 
From | �û��ĵ��������ַ 
Host | ������Դ���ڷ����� 
If-Match | �Ƚ�ʵ���ǣ�Etag�� 
If-Modified-Since | �Ƚ���Դ�ĸ���ʱ�� 
If-None-Match | �Ƚ�ʵ���ǣ���If-Match�෴�� 
If-Range | ��Դδ����ʱ����ʵ��Byte�ķ�Χ���� 
If-Unmodified-Since | �Ƚ���Դ�ĸ���ʱ�䣬��If-Modified-Since�෴ 
Max-Forwards | ����������� 
Proxy-Authorization | ����������Ҫ��ͻ��˵���֤��Ϣ 
Range | ʵ����ֽڷ�Χ���� 
Referer | ��������URI��ԭʼ��ȡ�� 
TE | �����������ȼ� 
User-Agent | HTTP�ͻ��˳������Ϣ 

### ��Ӧͷ���ֶ�

��Ӧ����ʹ�õ�ͷ���ֶΣ���������Ӧ�ĸ������ݡ�

ͷ���ֶ��� | ˵��
- | :-: 
ͷ���ֶ��� | ˵�� 
Accept-Ranges | �Ƿ�����ֽڷ�Χ���� 
Age | ������Դ��������ʱ�� 
Etag | ��Դ��ƥ����Ϣ 
Location | ��ͻ����ض������ƶ�URI 
Proxy-Authenticate | �����������Կͻ��˵���֤��Ϣ 
Retry-After | ���ٴη��������ʱ��Ҫ�� 
Server | ��������������Ĺ�����Ϣ 
WWW-Authenticate | �������Կͻ��˵���֤��Ϣ 



# 13. HTTP��ȱ���ƿ��
* ���������ı���ͨ�����ݿ��ܱ�����

* ����֤ͨ��˫�������ݿ�����αװ

* �޷�֤�����������Կ�����۸�

* һ��������ֻ�ɷ�һ������

* ��ͷ����

* ����ֻ���ɿͻ��˷��𣬿ͻ��˲��ɽ�����Ӧ֮���ָ��

* �������Ӧ���ײ�δ��ѹ���ͷ��ͣ��ײ���ϢԽ���ӳ�Խ��

* �����߳����ײ����������֮���ײ��󲿷��ֶζ�δ�ı䣬�˷���Դ

* ��ѡ������ѹ����ʽ����ǿ��ѹ������

**���ص�12�������������ı���ͨ�����ݿ��ܱ�����: ����������͸���C����̽����̽���ݿ���˺����롣**

**ǰ�����밲ȫ��أ��������봫���������**

# 14. HTTP/2
The focus of the protocol is on performance; specifically, end-user perceived latency, network and server resource usage. One major goal is to allow the use of a single connection from browsers to a Web site.


��Ҫ����:

* �����Ʒ�֡

* ��·����(һԴһ��TCP��һTCP�������һ��Ӧ��������ͷ����)

* ��������(ӵ�����������ȼ�����)

* ��������ͣ�
һ����������Ӧ��һ��request message��Ӧ���response message��������һ�� request ��Ӧһ��response������ǰ����client�ȷ���request����

* ͷ��ѹ����

* ���߻�����

* TLS����

### 14.1 �����Ʒ�֡
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_BinaryFraming.png)
HTTP 2.0�����ص㣺 ����Ķ�HTTP �����壬HTTP ������״̬�롢URI ���ײ��ֶΣ��ȵ���Щ���ĸ�����һ��������ȴ��������ͻ����һ����׼���������ƣ��Ľ��������ܣ�ʵ�ֵ��ӳٺ͸�����������֮���Խ�2.0�������������Ķ����Ʒ�֡�㡣

��Ȼ��Ҫ��֤HTTP�ĸ��ֶ��ʣ��������ײ�������Ӱ�죬�Ǿ���Ҫ**��Ӧ�ò�(HTTP2.0)�ʹ����(TCP or UDP)֮������һ�������Ʒ�֡�㡣**

�ڶ����Ʒ�֡���ϣ�HTTP 2.0 �Ὣ���д������Ϣ�ָ�Ϊ��С����Ϣ��֡,�������ǲ��ö����Ƹ�ʽ�ı��� ������HTTP1.x��**���ص�13�����ײ���Ϣ�ᱻ��װ��Headers֡��request body���װ��Data֡���档**

### 14.2 ����������Ϣ��֡
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_Stream.png)

HTTP/2��HTTPЭ��ͨ�ŷֽ�Ϊ�����Ʊ���֡�Ľ�������Щ֡��Ӧ���ض��������е���Ϣ��������Щ����һ��TCP�����ڸ��á�����HTTP/2Э�������������ܺ������Ż��Ļ�����


**���ص�14����ÿ������������Ϣ����ʽ���ͣ�����Ϣ��һ����֡���**

HTTP2.0����ͨ�Ŷ�����һ��TCP��������ɡ�HTTP 2.0 �� HTTP Э��ͨ�ŵĻ�����λ��СΪһ��һ����֡����Щ֡��Ӧ���߼����е���Ϣ��


**���ص�15����HTTP���ܵĹؼ����ڵ��ӳٶ����Ǹߴ�����**�����HTTP ���ӵ�ʱ�䶼�̣ܶ�������ͻ���Եģ���TCP ֻ�ڳ�ʱ�����Ӵ���������ʱЧ�ʲ���ߡ�HTTP 2.0 ͨ������������������ͬһ�����ӣ����Ը���Ч��ʹ��TCP ���ӣ��øߴ���Ҳ�������ķ�����HTTP������������

### 14.3 ��������Ӧ����
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_multiplexing.png)

�ͻ��˺ͷ��������Խ�HTTP��Ϣ�ֽ�Ϊ����������֡��Ȼ��(��������)�������ͣ����������һ�˰�����������װ����

**���ص�16������Щ֡���������ͣ�Ȼ���ٸ���ÿ��֡�ײ�������ʶ��������װ��**

**��·���ã�����˶�ͷ����**

#### ���ص�17��������߻���ȣ��ŵ���Client���ð�˳��һ�δεķ������󣬿��Խ�����������

### 14.4 ���������ȼ�
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_priority.png)

������������ϵ��Ȩ�ص�����ÿͻ��˿��Թ����ʹ��ݡ����ȼ���������������������ν�����Ӧ��������������������ʹ�ô���Ϣͨ������CPU���ڴ��������Դ�ķ����趨���������������ȼ�������Դ���ݿ���֮�󣬴����������ȷ���������ȼ���Ӧ�����ŷ�ʽ�������ͻ��ˡ�

**���ص�18��**���������һ����ҳ����ҳ������100��ͼƬ�����Ӧ������ͼ����ôʹ�����ȼ����ȼ��س���100�ŵ�����ͼ��Ȼ���ټ���ԭͼ��

### 14.5 ������
��������һ����ֹ���ͷ�����շ����ʹ������ݵĻ��ƣ����ⳬ�����ߵ��������������

��**TCPЭ���������**���ƣ�������HTTP/2��������һ��TCP�����ڸ��ã�TCP�����ƼȲ�����ϸ��Ҳ�޷��ṩ��Ҫ��Ӧ�ü�API�����ڸ����������Ĵ��䡣

**Ӧ�ò�������**�������������ȡһ�����ض���Դ��ͨ���������������ƴ��ڼ�СΪ������ͣ��ȡ���Ժ����лָ���
**���磬ֻ�Ȼ�ȡͼƬԤ��Ȼ����ͣ����ͼƬ��������JS�ű����ٻָ�ͼƬ���ء�**

**���ص�19������Ӧ�ò�����������������ͣ��������һ��stream������ͣ��**

### 14.6 ���������
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_Push.png)

���������Զ�һ���ͻ��������Ͷ����Ӧ���������˶�����������Ӧ���������������ͻ������Ͷ�����Դ��������ͻ�����ȷ������

### 14.7 ͷ��ѹ��
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/HTTP_headerCompress.png)

ͨ����̬Huffman����Դ���ı�ͷ�ֶν��б��룬�Ӷ���С�˸�������Ĵ�С��Ҫ��ͻ��˺ͷ�����ͬʱά���͸���һ������֮ǰ�����ı�ͷ�ֶε������б�����֮ǰ�����ֵ������Ч���롣

## 15 HTTPS
��ȫ�����θ�
����+��֤+�����Ա���
SSL vs TLS������ȡ��ǰ��

## 16 RESTful

RESTful, ȫ��Representational State Transfer����һ����Ʒ���ṩ��һ�����ԭ���Լ����������Ҫ���ڿͻ�����������Ľ�����**���ص�20����ͨ�׵Ľ���URL��λ��Դ����HTTP���ʣ�GET,POST,DELETE,DETC����������**

**���ص�21��**��
* Representational��ĳ�ֱ�����ʽ��������JSON��XML��JPEG�ȣ�

* State Transfer��״̬�仯��ͨ��HTTP����ʵ�֡�


**���ص�22��������APIʱҪ���ص�һ�ֹ���/�����Ҫ��������� RESTful API��REST��������ӿڡ���һ������Ĺ淶��ָ��ԭ�򣬵�Ҳ���ǽ�����**

* GET ������ȡ��Դ��

* POST �����½���Դ��Ҳ�������ڸ�����Դ����

* PUT ����������Դ��

* DELETE ����ɾ����Դ��


**���ص�23����Server��Client֮�䴫��ĳ��Դ��һ��������ʽ��������JSON��XML�����ı���������JPG��WebP����ͼƬ�ȡ�**

ǰ�����JSON��XML������Ǵ�����Դ�����ݽṹ������һ��������HTML�ĵ���������һ������ҳ��϶��ɶ����Դ���ɡ�


�� HTTP Status Code����Server��״̬��Ϣ��

**���ص�24����ΪʲôҪ��RESTful�ṹ��**
��ǰ��������http��post��get��restful���������delete put patch��Щmethod����������������ͨ��post���ϲ���action=delete��ʵ��ɾ��������



�ο����ף�
https://www.cnblogs.com/icelin/p/3974935.html
https://blog.csdn.net/qq_28885149/article/details/52922107
https://blog.csdn.net/u010369338/article/details/65627999
https://blog.csdn.net/u011904605/article/details/53012844
https://www.zhihu.com/question/28557115/answer/48094438