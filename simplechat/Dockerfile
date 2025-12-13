# 1. Dùng nền tảng Java 17 (hoặc 21 tùy máy em, nhưng 17 là chuẩn nhất)
FROM eclipse-temurin:21-jdk-alpine

# 2. Tạo vùng chứa tạm
VOLUME /tmp

# 3. Copy file .jar đã build xong vào trong Docker
# Lưu ý: Lệnh này sẽ tìm bất kỳ file .jar nào trong folder target
COPY target/*.jar app.jar

# 4. Chạy ứng dụng
ENTRYPOINT ["java","-jar","/app.jar"]