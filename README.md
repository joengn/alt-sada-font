# alt-sada-font

File tải về của font **Sa Đà** (bản dùng thử) cho trang https://fonts.studioalt.work/sada/.

Nút Download trên trang luôn trỏ tới bản mới nhất:
`https://github.com/joengn/alt-sada-font/releases/latest/download/AltSADATrial.zip`

## Cập nhật bản mới

**Cách nhanh:** chạy trong Terminal (script nằm ngoài repo, trong `AltType/SADA/Publish/`)

```bash
~/Documents/Claude/AltType/SADA/Publish/update.sh
```

Script lấy file `.zip` mới nhất trong `AltType/SADA/Release`, đổi tên thành `AltSADATrial.zip`,
ghi phiên bản gốc vào `VERSION`, rồi commit + push. Khoảng 1 phút sau GitHub Actions tạo Release
mới (tự đánh số) và trang web tự tải bản đó — không cần sửa code hay deploy lại website.

**Cách thủ công:** chép file mới vào thư mục này với đúng tên `AltSADATrial.zip`,
rồi commit + push lên `main` (GitHub Desktop cũng được).

## Lưu ý
- Luôn giữ đúng tên **`AltSADATrial.zip`**.
- Số phiên bản tự đánh trên GitHub: mỗi lần ZIP thay đổi là một Release mới. Nếu tên thư mục trong ZIP (`AltSADATrial-1.000/` → `1.000`) mới hơn Release gần nhất thì dùng số đó, nếu không thì tăng 0.001 (`v1.000` → `v1.001` → `v1.002`…). File ZIP giữ nguyên tên gốc như lúc build.
- Repo phải để **Public** thì người ngoài mới tải được.
- Dòng "ZIP / … KB · v…" trên trang tự cập nhật theo Release mới nhất.
