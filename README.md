# richbiotech-leave
ลงวันลา/วันหยุด พนักงาน
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ระบบลงวันหยุดพนักงาน</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="logo">MyCompany</div>
        <div class="user-profile">
            <span>ยินดีต้อนรับ, คุณสมชาย</span>
            <img src="avatar.png" alt="Avatar">
        </div>
    </header>

    <main>
        <section class="overview">
            <div class="card">
                <h3>วันลาคงเหลือ</h3>
                <p>10 วัน</p>
            </div>
            <div class="card">
                <h3>พนักงานที่ลาวันนี้</h3>
                <p>2 คน</p>
            </div>
            <div class="card">
                <h3>คำขอรออนุมัติ</h3>
                <p>1 รายการ</p>
            </div>
        </section>

        <section class="calendar-section">
            <h2>ปฏิทินวันหยุดทีม</h2>
            <div id="calendar"></div>
        </section>
        
        <section class="request-table">
            <h2>รายการคำขอลา</h2>
            <table>
                <thead>
                    <tr>
                        <th>ชื่อพนักงาน</th>
                        <th>ประเภทการลา</th>
                        <th>วันที่</th>
                        <th>สถานะ</th>
                        <th>จัดการ</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>สมหญิง</td>
                        <td>ลาพักร้อน</td>
                        <td>18/09/2025 - 20/09/2025</td>
                        <td><span class="status pending">รอดำเนินการ</span></td>
                        <td><button class="approve">อนุมัติ</button> <button class="reject">ปฏิเสธ</button></td>
                    </tr>
                </tbody>
            </table>
        </section>
    </main>
</body>
</html>
/* Basic Styling */
body {
    font-family: 'Sarabun', sans-serif;
    margin: 0;
    background-color: #f4f7f6;
    color: #333;
}
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #ffffff;
    border-bottom: 1px solid #ddd;
}
main {
    padding: 2rem;
}
.overview {
    display: flex;
    gap: 1.5rem;
    margin-bottom: 2rem;
}
.card {
    background-color: #fff;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    flex-grow: 1;
}
/* Table Styling */
table {
    width: 100%;
    border-collapse: collapse;
    background-color: #fff;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
th, td {
    padding: 1rem;
    text-align: left;
    border-bottom: 1px solid #ddd;
}
.status.pending {
    background-color: #ffc107;
    color: #333;
    padding: 0.25rem 0.5rem;
    border-radius: 12px;
    font-size: 0.8em;
}
