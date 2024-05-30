# JMeter
<h1>Kiểm tra hiệu năng trang web</h1>
<h2>Mục tiêu:</h2>
<ul>
  <li>Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://canvas.phenikaa-uni.edu.vn/</li>
  <li>Chạy kịch bản kiểm tra và ghi lại kết quả.</li>
  <li>Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.</li>
  <li>Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.</li>
</ul>
<h2>Kịch bản kiểm tra:</h2>
<ul>
  <li>Thread Group:
    <ul>
      <li>Số lượng thread: 1000</li>
      <li>Thời gian chạy: 30 giây</li>
      <li>Ramp-up period: 10 giây</li>
    </ul>
  </li>
    <li>HTTP Request:
    <ul>
      <li>URL: https://canvas.phenikaa-uni.edu.vn/</li>
      <li>Method: GET</li>
      <li>Content encoding: UTF-8</li>
    </ul>
  </li>
    <li>Listeners:
    <ul>
      <li>View Results Tree</li>
      <li>Aggregate Report</li>
    </ul>
  </li>
</ul>
<h2>Kết quả kiểm tra:</h2>

![image](https://github.com/sangtvs/JMeter/assets/124127082/40e91cad-b9e9-4c37-bf13-c48933a466dc)

![image](https://github.com/sangtvs/JMeter/assets/124127082/8018e438-3718-48e8-967a-0de11e95da7d)
<h2>Phân tích kết quả kiểm tra</h2>
    <ul>
      <li>Số lượng yêu cầu thành công: 999/1000 = 99,9%</li>
      <li>Số lượng yêu cầu thất bại: 1/1000 = 0,1%</li>
    </ul>
<h2>Kết luận: Trang web https://canvas.phenikaa-uni.edu.vn/ có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (99,9%), số lượng yêu cầu thất bại rất thấp (0,1%).</h2>
