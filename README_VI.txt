BKOOsjkj VIP - mã nguồn Android mẫu
====================================

Đây là mã nguồn ứng dụng Android quản lý/chọn tệp, chưa phải APK đã build.
Ứng dụng không áp dụng patch vào game. Việc tích hợp patch cần APK gốc, kiểm tra tương thích và quyền sử dụng.

Build trên Android bằng Termux:
1. Cài Termux từ nguồn chính thức và cài JDK + Gradle:
   pkg update
   pkg install openjdk-17 gradle
2. Giải nén BKOOsjkj_VIP_App.zip vào thư mục dễ truy cập.
3. Vào thư mục dự án (nơi có settings.gradle), chạy:
   gradle assembleDebug
4. Nếu build thành công, APK nằm tại:
   app/build/outputs/apk/debug/app-debug.apk

Nếu Android SDK chưa được cấu hình trong Termux, Gradle sẽ báo thiếu SDK. Khi đó cần cài/cấu hình Android SDK phù hợp trước; dự án này không kèm SDK hay Gradle wrapper.
