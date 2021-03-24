# Cách cài đặt module pagespeed đơn giản nhất đến trẻ con cũng có thể làm được trên CentOS 7
Hiện nay có 2 web server thông dụng nhất đó là nginx và apache. Bài hôm nay sẽ hướng dẫn cách cài đặt module pagespeed của google cho cả 2 web server
# 1. Cài đặt module pagespeed cho apache
Đầu tiên thì máy đã được cài apache làm web server đã. Cách kiểm tra: Nhập lệnh **systemctl status httpd** để xem thử đã cài đặt apache chưa. Nếu chưa thì cài đi nhé.
Module pagespeed trong apache đuôc gọi là mod_pagespeed. Có thể được cài đặt một cách cực kì đơn giản qua các bước sau:
1. Kiểm tra thử wget đã được cài đặt chưa. Chưa được cài đặt thì cài đi nhé. Sau đó làm theo hướng dẫn sau:
  > yum íntall at -y (Package cần cho khi cài đặt module pagespeed)
  >
  >  cd /tmp
  >
  > wget https://dl-ssl.google.com/dl/linux/direct/mod-pagespeed-stable_current_x86_64.rpm
  > 
  > rpm -U mod-pagespeed-*.rpm

THế là ta đã cài đặt xong module pagespeed cho apache. Ta có thể kiểm tra bằng cách bật trình duyệt lên vào chế độ Develop Mode cách nhấn phím F12. Trong tab network ta có thể thấy được mode_pagespeed được gọi.  
 https://i.imgur.com/nqT3o8J.png
