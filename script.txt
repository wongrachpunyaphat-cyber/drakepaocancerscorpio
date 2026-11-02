// เปิดแอปเมื่อกดไอคอน
function openApp(appId) {
    // ซ่อนหน้า Home
    document.getElementById('home-screen').classList.remove('active');
    
    // แสดงแอปที่เลือก
    document.getElementById(appId).classList.add('active');
}

// กลับหน้า Home
function goHome() {
    // ปิดแอปทั้งหมด
    const apps = document.querySelectorAll('.app-page');
    apps.forEach(app => app.classList.remove('active'));
    
    // เปิดหน้า Home
    document.getElementById('home-screen').classList.add('active');
}
