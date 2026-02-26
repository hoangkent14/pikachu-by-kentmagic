/* Tìm đoạn này trong CSS và sửa lại */
canvas {
    /* ... các style khác ... */
    max-width: 95vw; /* Cho phép giãn theo màn hình thay vì fix 1200px */
    max-height: 80vh;
}
.ribbon-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(90px, 1fr));
    gap: 4px;
    max-width: 800px; /* Thêm dòng này để giới hạn độ dài */
    margin: 0 auto;   /* Căn giữa */
}
Nếu muốn thu ngắn thanh "Stats" (Chứa Level, Điểm, Thời gian...)
Tìm đến class .ribbon-stats. Thanh này đang sử dụng display: grid. Bạn có thể giới hạn độ dài của nó bằng cách thêm max-width:
.ribbon.ribbon-actions {
    /* ... các thuộc tính cũ ... */
    width: 80% !important; /* Đổi 100% thành 80% hoặc 600px tùy ý */
    margin: 0 auto !important; /* Để thanh này nằm căn giữa màn hình */
}
Nếu muốn thu ngắn thanh "Action" (Chứa các nút Game mới, Gợi ý...)
Tìm đến class .ribbon-actions (khoảng dòng 27-28 trong đoạn code bạn gửi).
Hiện tại nó đang có width: 100% !important;. Bạn hãy đổi thành một con số cụ thể và thêm margin: 0 auto; để nó nằm giữa:
