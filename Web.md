# Web

## 1��ʲô��Web��
��ά��(��дΪWWW��Web)��һ����Ϣ�ռ䣬�����ĵ�������Web��Դ��ͳһ��Դ��λ����URL)��ʶ��ͨ�����ı����ӻ��������ҿ���ͨ�����������ʡ�

## 2��Web�ĺ��ļ�����

* html�����峬�ı��ĵ��Ľṹ�͸�ʽ

* http���涨�ͻ��˺ͷ�������ͨ��

* url��������Դ���������ϵ�λ��

�����ļ��������棬Session�ȵȣ����Ƕ�������ϵ�����ƣ����Ľṹ����δ�䡣ֻҪʵ���������������ļ����㣬�Ϳ��Թ���һ����̬��ҳ��

**�������������������ļ����㣺**
Web framework����ĵļ��������routing��Web Server�ܹ��������������url�ҵ���Ӧ�ľ�̬�ļ����߿�ִ���ļ���Ȼ�󷵻���Դ���ͻ��ˡ����ڿͻ��˺�Web Server��ͨ����ͨ��������/����:�˿ڡ�

* html���ҵ���̬htmlҳ����߶�̬����htmlҳ�棬htmlҳ�������ͼƬ��json���������͵���Դ
* http��Web Server����˽��տͻ���ͨ��httpЭ�鴫�ݹ��������ݣ����ݿ����Ǳ����ı������͡�Ȼ������ݽ�����������Ӧ����Ӧ��
* url��routing·�ɣ�Web Server�ҵ���url��Ӧ����Դ��

## 3��Web�ķ�չʷ
* 1990��HttpЭ�鵮����12�·�����һ����ҳ�����WorldWideWeb�͵�һ��Web������CERN httpd
* 1993��CGI����
* 1995��Apache Web��������JavaScript������Html2.0����
* 1996��Http/1.0����
* 2002��FireFox���������
* 2003��WSGI1.0����
* 2004��Nginx����
* 2005��AJAX����
* 2006��JQuery����
* 2014��HTML5.0����

## 4��Web Server �� HTTP Server
* Web Server��Web����������Web������������һ��HTTP daemon���ػ������̣�����url���������ʱ�򣬸�Web�������ܹ�����url�ѷ���������url��Ӧ�����ݷ��ظ��ͻ����������
* HTTP Server��HTTPЭ�������չ/��ǿЭ���֧���£�Web���ܹ���Ϊһ����Ϣ�ռ䡣����Ҳ����˵HTTP Server��Web Server

## 5��CGIЭ�飨Common Gateway Interface��
* CGI��ͨ�����ؽӿ�
* CGI��Ŀ�ģ�ʵʱ��ִ��ĳЩ���������̬����
* CGIЭ�飺�涨Web Server�Ϳ������ɶ�̬���ݵĿ�ִ�г�����ν��н���

  ��ȻCGIЭ���ǹ涨Web Server�Ϳ�ִ�г�����н�������ô���Ǿ���ҪWeb Server֧��CGIЭ�顣ǰ�������Ѿ�֪��Web Server��Apache��Nginx����ôͨ�����CGIģ����߲����mod_php,mod_python������CGI���Ϳ�����Apache����Nginxִ��ĳЩ��ִ�г��򣨱���PHP�ű�����Python�ű��������ɶ�̬ҳ�档

  ��Web Server�����CGIģ������󣬽�����Ҫ����CGI�����磺Web Serverִ�п�ִ�е��ļ���Ҫ�����ĸ�Ŀ¼�£����ڣ�/cgi/bin��Ŀ¼�£�Web ServerҪִ���������͵��ļ���shell��PHP��Python��C/C++����
  
  
## 6��Apache ʹ��CGI����py�ļ�
#### ��װpython��apache2

 ``` apt-get install python```  ��װPython,Ĭ��2.7

 ``` apt-get install apache2``` ��װapache2��Ĭ�ϸ�Ŀ¼��/var/www/html ��

#### ����CGI

``` a2enmod cgi```  ����CGIģ��

��������������˵����������CGI

```
Your MPM seems to be threaded. Selecting cgid instead of cgi.
 Enabling module cgid.
 To activate the new configuration, you need to run:
 service apache2 restart
```


������CGIģ���Ĭ������£�CGI�ű�������"/usr/lib/cgi-bin"Ŀ¼��ִ�С�

����ֻҪ��"/usr/lib/cgi-bin"Ŀ¼�´���demo_py.py�ļ��󣬿ͻ��˷���"http://(Apache2 Server)/cgi-bin/demo_py.py"��Apache�ͻ�ִ��demo_py.py�ļ����������ݷ��ظ��ͻ��ˡ�

#### Writing a CGI program
��дdemo_py.py�ļ�������"/usr/lib/cgi-bin"Ŀ¼�£�
```
#!/usr/bin/python

print('Content-type: text/html\n\n')
print('Hello, World.')
```

* ��һ�нű���������·��������Apache���������������е��κ�shell�����ó������ͨ�����ļ��ṩ���ڸ�λ���ҵ��Ľ�������ִ��

* ����������������۵���������������������������س����з���

* ����������ַ���

#### ����Ȩ��
�����������������ն���һ�����С�Ҳ����˵��������������ʱ�������Է���Ȩ�û���Ȩ�����С�������Ҫ���ļ�����Ȩ�ޡ�

```
chmod 705 /usr/lib/cgi-bin/demo_py.py
```
#### ���ͻ��˷��ʼ���:http://www.example.com/cgi-bin/demo_py.py

#### ���⻰��STDIN��STDOUT
�������Ϳͻ���֮�������ͨ��ͨ����׼���루STDIN���ͱ�׼�����STDOUT�����С����������ճ�����£� STDIN��ζ�ż��̻���򱻸���ִ�е��ļ���STDOUT ͨ����ζ�ſ���̨����Ļ��

��POST����ʱ�����е����ݽ��������һ������ĸ�ʽ�����ݸ�CGI������STDIN��Ȼ���������������Լ��̻��ļ�һ����������ݡ�

### 6.2 ǰ����ܵ���Ĭ��Ŀ¼���������ʹ��Ĭ�ϵ�cgi-binĿ¼��ʹ���Լ�������Ŀ¼
���磺����cgi�ű���"/var/www/html/cgi-enabled"Ŀ¼��

#### ��conf-availableĿ¼���½�һ��cgi-enabled.conf�ļ�
```vi /etc/apache2/conf-available/cgi-enabled.conf``` 

cgi-enabled.conf�ļ����ݣ�
```
<Directory "/var/www/html/cgi-enabled">
    Options +ExecCGI
    AddHandler cgi-script .py .cgi .pl
</Directory></pre>
```

#### �����½���cgi-enabled.conf�ļ�
```a2enconf cgi-enabled```

#### ����"/var/www/html/cgi-enabled"Ŀ¼,���½�һ�������ļ�demo_py.py
```mkdir /var/www/html/cgi-enabled```

```vi demo_py.py```

demo_py.py�ļ�����Ϊ��

```
#!/usr/bin/python

print "Content-type: text/html\n\n"
print "<html>\n<body>\n"
print "<div style=\"width: 100%; font-size: 40px; font-weight: bold; text-align: center;\">\n"
print "CGI Test Page"
print "\n</div>\n"
print "</body>\n</html>\n"
```

#### �޸�Ȩ��
```
chmod 705 /var/www/html/cgi-enabled/demo_py.py
```

### 6.3 ��ʹ��a2enmod����CGIģ��
#### 1�� ��httpd.conf�ļ���ȷ�� LoadModule ָ��û�б�ע�͵�
```LoadModule cgid_module modules/mod_cgid.so```

#### 2�� ScriptAliasָ��
����ApacheΪCGI����Ԥ����һ���ض���Ŀ¼��Apache��ٶ����Ŀ¼�е�ÿ���ļ�����һ��CGI���򣬲��ҵ��ͻ���������ض���Դʱ������ִ������

�κζ�/cgi-bin/��ʼ����Դ����Ӧ�ôӸ�Ŀ¼"/usr/local/apache2/cgi-bin/"��Ѱ�ң����URL http://www.example.com/cgi-bin/test.pl ������Apache������ִ��"/usr/local/apache2/cgi-bin/test.pl"���ļ����������������Ȼ���ļ�������ڣ����ҿ�ִ�У������ض���ʽ�������������Apache�����ش�����Ϣ��

#### 3��Optionsָ�AddHandlerָ��

�����ָ�����Apache����ִ��CGI�ļ�

```
<Directory "/usr/local/apache2/htdocs/somedir">
    Options +ExecCGI
</Directory>
```

AddHandlerָ����߷����������д���cgi��pl��py��չ�����ļ���ΪCGI����

```AddHandler cgi-script .cgi .pl .py```

## 7��CGI������ͼ��ִ�в��裺
![](https://raw.githubusercontent.com/SkewwG/architecture/master/Picture/CGI.png)

* �ͻ��˷��������Web Server��Apache��

* Apache���յ��ͻ��˷��͵����󣬽������ݹ��������ݡ�����Ƕ�̬������ô�ͻ������ű���������������CGI�Ļ���������

* �ű������������󣬾ͻ��ڸղŴ��ݹ�����CGIĿ¼���ҵ��ͻ���������Ǹ��ļ���Ȼ��ȥִ�иýű���ִ��������ݷ��ظ�Apache����ֱ�ӷ��ظ��ͻ��ˡ�


## 8��WSGI
WSGI��Web Server Gateway Interface��Web ���������ؽӿڣ�����[Python](http://lib.csdn.net/base/python "Python֪ʶ��")�������������Web��������WebӦ�ó���֮�����֮���**ͨ�ýӿڱ�׼**��

WSGI�����ı����Ǹ���Python Web��ܸ���Ϊ�������е�ʹ��Pythonʵ��Server���ܣ��е���FastCGl֮�������Э�����Python��Ϊ����ͨ�û���ѡ����ʱ����̫�����ƣ�ҲΪ�˸���serer������framework������

## 9.Apache
��NCSA httpd 1.3�ݽ�������Web Server

* mod_python��ͣ��

* mod_fastcgi�е����⣬�г�ռ����С

* mod_fcgid���ڴ���mod_ fastcgi�����flupʹ��

* mod_wsgi֧��Ƕ��Apache Server�����ж������ػ�������FastCGl���ʹ��

## 10.Nginx
Nginx�����ĳ�����Ϊ�˽��C10k���⣬�����첽�¼������ܹ�,�ֽ����Ѽ�HTTP Server,  Reverse Proxy Server,  Mail Proxy,  Server,  Generic TCP/UDP Proxy Server��һ����������HTTP Server���������(����ת����HTTP��������������ؾ�����)

## 11.Web Application&Web Framework
* ����ʹ��Web Frameworkȥ����Web Application

* Web Application�������ɶ�̬���ݣ������������ؾ�̬���ݡ�����Flask��app����Web Application

* Web Framework��Ҫ�㶨����MVC�ܹ���routing��session��authentication��security�ȷ��棬Ϊ���渴�Ӻ͹�ģ�Ӵ��Web Application�����ṩ����������Django��Flask��Tornado


�ο����ϣ�
https://httpd.apache.org/docs/2.4/howto/cgi.html
https://www.server-world.info/en/note?os=Ubuntu_14.04&p=httpd&f=2
