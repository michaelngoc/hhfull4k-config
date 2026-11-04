# hhfull4k-config

File cấu hình có chữ ký cho app HHFULL4K (`config.signed.json`, chữ ký Ed25519, keyId `5b3a4a3fda8d82c7`).

App đọc file này khi không gọi được máy chủ chính, để biết địa chỉ máy chủ mới. File chỉ chứa thông tin công khai (địa chỉ máy chủ, địa chỉ phim, cờ tính năng) và có hạn tối đa 30 ngày. App kiểm chữ ký trước khi dùng, nên sửa tay file này sẽ bị app bỏ qua.

Cập nhật: chạy `npm run config:export -- --days 30` ở backend (xem `backend/docs/CONFIG-KY-SAN.md` trong repo chính), thay file ở đây và trên NAS, khoảng 3 tuần một lần.
