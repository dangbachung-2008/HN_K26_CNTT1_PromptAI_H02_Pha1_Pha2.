# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 09
- **Họ tên:Đặng bá chung**
- **Lớp:Cntt1**
- **Link repository Pha2:https://github.com/dangbachung-2008/HN_K26_CNTT1_PromptAI_H02_Pha1_Pha2.**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):chatGPT**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt chỗ workshop ra JSON

**KET QUA AI**

```text
[
  {
    "ma_lop": "NANTAY",
    "ngay_hoc": "2026-12-13",
    "nguoi_lon": 2,
    "tre_em": 1,
    "ca_hoc": "chieu",
    "ghi_chu": null
  },
  {
    "ma_lop": "BANXOAY",
    "ngay_hoc": "2027-01-10",
    "nguoi_lon": 3,
    "tre_em": 0,
    "ca_hoc": null,
    "ghi_chu": "1 người bị đau cổ tay"
  },
  {
    "ma_lop": "VEGOM",
    "ngay_hoc": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "ca_hoc": "sang",
    "ghi_chu": "1 bạn đi xe lăn"
  }
]
```

**Link trò chuyện:https://chatgpt.com/share/6b07e560-e31c-83ec-81f0-73c642f7add5**

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
Bước 1: Tiền người lớn
- Có 5 người lớn.
- Giá BANXOAY: 550.000 đồng/người.
- Phép tính: 5 × 550.000 = 2.750.000 đồng.
Bước 2: Tiền trẻ em
- Trẻ 8 tuổi: tính 70% giá người lớn.
  - 550.000 × 70% = 385.000 đồng.
- Trẻ 12 tuổi: tính 70% giá người lớn.
  - 550.000 × 70% = 385.000 đồng.
- Bé 4 tuổi: dưới 6 tuổi, đi kèm và không làm sản phẩm nên miễn phí.
- Tổng tiền trẻ em: 385.000 + 385.000 + 0 = 770.000 đồng.
Bước 3: Tiền học (người lớn + trẻ em)

2.750.000 + 770.000 = 3.520.000 đồng.

Bước 4: Giảm giá nhóm
- Nhóm có 5 người lớn, đủ điều kiện giảm 5%.
- Số tiền được giảm: 3.520.000 × 5% = 176.000 đồng.
- Tiền học sau giảm: 3.520.000 − 176.000 = 3.344.000 đồng.
Bước 5: Phí nung và giao
- Có 4 sản phẩm cần nung và giao.
- Phí: 80.000 đồng/sản phẩm.
- Phép tính: 4 × 80.000 = 320.000 đồng.
- Phí này không được giảm giá.
Bước 6: Tổng tiền

3.344.000 + 320.000 = 3.664.000 đồng.

[RESULT: 3.664.000 đồng]
```

**Link trò chuyện:https://chatgpt.com/share/6b07e5fc-8b98-83ec-912f-b4cee7b7fd8f**

### b) Kiểm tra kết quả AI

kết quả AI cho là đúng với kết quả mình tính 

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "HONG_SAN_PHAM": {
    "so_san_pham": 5,
    "muc_den_bu_moi_san_pham": 150000,
    "tong_den_bu": 750000,
    "xu_ly": "Hoàn 750.000 đồng cho 5 sản phẩm bị nứt vỡ",
    "phe_duyet": "Cần Quản lý xưởng duyệt trước khi gửi khách"
  },
  "GIAO_TRE": null,
  "HUONG_DAN": null,
  "KHAC": null
}
```

**Link trò chuyện:https://chatgpt.com/share/6b07e672-904c-83ec-b352-cc63a78b24f6**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Tiêu chí	Điểm	Minh chứng	Đề xuất sửa

| Đúng thông tin (5 điểm) | 1/5 | - Sai giá: "Lớp vẽ gốm bên em 200k thôi nè" — Giá chuẩn là 250.000 đồng/người lớn. Sửa: "Lớp vẽ gốm có giá 250.000 đồng/người lớn."
```

**Link trò chuyện:https://chatgpt.com/share/6b07e6be-359c-83ec-90bd-a16aac3a588b**
