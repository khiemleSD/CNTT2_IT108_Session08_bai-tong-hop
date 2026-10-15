# Ghi chú ôn tập

## Phần 4. Bẫy cú pháp

Đoạn bạn cùng nhóm gửi:

```markdown
| Tính năng | Trạng thái |
| Tra cứu lịch học | Xong |
| Push notification | Đang làm |

-[x] Tra cứu lịch học
-[ ] Push notification
```

Hai lỗi:

1. Bảng thiếu dòng phân cách `| --- | --- |` ngay dưới hàng tiêu đề, nên parser không nhận ra bảng và hiện thành các dòng chữ có dấu `|`.
2. Task list thiếu dấu cách sau `-` (`-[x]`, `-[ ]`), nên không thành ô tick mà hiện nguyên ký tự.

Đoạn đã sửa:

```markdown
| Tính năng | Trạng thái |
| --- | --- |
| Tra cứu lịch học | Xong |
| Push notification | Đang làm |

- [x] Tra cứu lịch học
- [ ] Push notification
```
