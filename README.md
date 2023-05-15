# VideoServer_Group20
Link source code tham khảo: https://github.com/superdesk/video-server

## Thành viên nhóm
- Nguyễn Thị Bích Liên - 20110335
- Đặng Nguyễn Thiên Đạt - 20110629

## **Ngôn ngữ sử dụng**
- Python

## **Môi trường**
_Cài đặt môi trường theo yêu cầu của các version sau_
- Python (>=3.6)
- FFmpeg
- MongoDB
- RabbitMQ

## **Cài đặt để phát triển**
**_LƯU Ý: Sử dụng virtualenv và pip để cài đặt các module python._**
Tại thư mục ta setup code

> **git clone https://github.com/superdesk/video-server.git**

Cài đặt máy chủ video để phát triển
LƯU Ý: virtualenv của bạn phải được kích hoạt

> **pip install -e video-server/[dev]**

## **Chạy máy chủ video để phát triển**
_Máy chủ video bao gồm hai phần chính: http api và celery workers._

Để bắt đầu một máy chủ http api dev:

1. Đặt biến env `FLASK_ENV` để phát triển trên Windows:

> set FLASK_ENV=developement

2. Chạy `python -m videoserver.app`
