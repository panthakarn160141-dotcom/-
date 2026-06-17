<!DOCTYPE html><html lang="th"><head>
<meta charset="utf-8">
<meta content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover" name="viewport">
<meta content="yes" name="apple-mobile-web-app-capable">
<meta content="default" name="apple-mobile-web-app-status-bar-style">
<meta content="#f8f9fb" name="theme-color">
<title>TechFix Manager - ระบบจัดการงานซ่อม</title>
<!-- PWA Tags -->
<link href="manifest.json" rel="manifest">
<link href="https://lh3.googleusercontent.com/aida/AP1WRLtYcBuvj-VYDxuvdI8xcqBOYeWV2dK8A7MTMvWWoCtDeLmmNuQocBl7c8trEvSM7kCIOTBPb5L1B-Z1qDk5SHYShBu2AmGOU3hwcU6vv6cWk1_WrewfUP71bWeCHyszy_Cp0R348y6JN69tuDavk8ed4MvDgYgdP1nVGD1LnXPKmFXU929NAqNfGG2sm58hwtTnklFmORpYmsTMH18QrWWCHVA08jhIfPNfoNKDgwM636uPiwPaBVs84SA" rel="icon" type="image/png">
<link href="https://lh3.googleusercontent.com/aida/AP1WRLsm2cpE6q4w6B30v3vbTbDj58te9JvDpO51onxlCdWZyG7U9K51tWwdvK7MDnDozzLBFdphbpwbL75ad5S3IxkxRa1bKufsVhV9o4OZ_MexFnvF8GL3B5mHWVKsrPOx0VNOGxX-pllWyJMM9Ddho23ak39bMPMIK7Q9GVbOnsBhkFIsfpMJb4i3B_aYW-7-lpKCRU7rLbTee76WgvkPU2GyXnudSbaS9dXojKBjujHmPKGqBaVt3efKd_gP" rel="apple-touch-icon">
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@400;500;600;700&amp;display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet">
<style>
        body {
            font-family: 'Be Vietnam Pro', sans-serif;
            background-color: #f8f9fb;
            -webkit-tap-highlight-color: transparent;
        }
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
        }
        .status-chip {
            padding: 4px 12px;
            border-radius: 9999px;
            font-size: 12px;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 4px;
        }
        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
        /* Mobile Safe Area Padding */
        .pb-safe {
            padding-bottom: env(safe-area-inset-bottom);
        }
        .pt-safe {
            padding-top: env(safe-area-inset-top);
        }
    </style>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "surface-variant": "#e1e2e4",
                        "surface-bright": "#f8f9fb",
                        "on-primary-fixed-variant": "#0040a2",
                        "tertiary-container": "#7d5200",
                        "tertiary": "#5e3c00",
                        "on-secondary-container": "#475a7e",
                        "error-container": "#ffdad6",
                        "secondary": "#4c5e83",
                        "surface-container-lowest": "#ffffff",
                        "primary-fixed": "#dae2ff",
                        "on-secondary": "#ffffff",
                        "surface-container-low": "#f3f4f6",
                        "on-tertiary-container": "#ffca81",
                        "on-primary-container": "#c4d2ff",
                        "on-primary": "#ffffff",
                        "on-error": "#ffffff",
                        "inverse-surface": "#2e3132",
                        "outline": "#737685",
                        "tertiary-fixed-dim": "#ffb950",
                        "secondary-container": "#bfd2fd",
                        "outline-variant": "#c3c6d6",
                        "surface-tint": "#0c56d0",
                        "on-background": "#191c1e",
                        "background": "#f8f9fb",
                        "error": "#ba1a1a",
                        "on-primary-fixed": "#001848",
                        "surface-dim": "#d9dadc",
                        "secondary-fixed": "#d7e2ff",
                        "on-secondary-fixed-variant": "#34476a",
                        "on-tertiary": "#ffffff",
                        "surface": "#f8f9fb",
                        "secondary-fixed-dim": "#b4c7f1",
                        "surface-container": "#edeef0",
                        "inverse-on-surface": "#f0f1f3",
                        "on-secondary-fixed": "#041b3c",
                        "on-tertiary-fixed-variant": "#624000",
                        "surface-container-high": "#e7e8ea",
                        "on-surface": "#191c1e",
                        "inverse-primary": "#b2c5ff",
                        "primary-fixed-dim": "#b2c5ff",
                        "on-tertiary-fixed": "#291800",
                        "on-error-container": "#93000a",
                        "primary-container": "#0052cc",
                        "primary": "#003d9b",
                        "on-surface-variant": "#434654",
                        "surface-container-highest": "#e1e2e4",
                        "tertiary-fixed": "#ffddb3"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.25rem",
                        "lg": "0.5rem",
                        "xl": "0.75rem",
                        "full": "9999px"
                    },
                    "spacing": {
                        "sm": "12px",
                        "touch-target": "48px",
                        "lg": "24px",
                        "md": "16px",
                        "margin-mobile": "16px",
                        "base": "8px",
                        "xs": "4px",
                        "xl": "32px",
                        "margin-desktop": "40px",
                        "gutter": "16px"
                    },
                    "fontFamily": {
                        "label-lg": ["Be Vietnam Pro"],
                        "headline-lg": ["Be Vietnam Pro"],
                        "body-md": ["Be Vietnam Pro"],
                        "headline-md": ["Be Vietnam Pro"],
                        "label-sm": ["Be Vietnam Pro"],
                        "body-lg": ["Be Vietnam Pro"],
                        "headline-lg-mobile": ["Be Vietnam Pro"]
                    },
                    "fontSize": {
                        "label-lg": ["14px", {"lineHeight": "20px", "letterSpacing": "0.5px", "fontWeight": "600"}],
                        "headline-lg": ["24px", {"lineHeight": "32px", "fontWeight": "700"}],
                        "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                        "headline-md": ["20px", {"lineHeight": "28px", "fontWeight": "600"}],
                        "label-sm": ["12px", {"lineHeight": "16px", "fontWeight": "500"}],
                        "body-lg": ["18px", {"lineHeight": "26px", "fontWeight": "400"}],
                        "headline-lg-mobile": ["22px", {"lineHeight": "28px", "fontWeight": "700"}]
                    }
                },
            },
        }
    </script>
</head>
<body class="bg-surface text-on-surface mb-24 md:mb-0 md:pl-[320px]">
<!-- Sidebar (NavigationDrawer) - Responsive Web -->
<aside class="hidden md:flex fixed left-0 top-0 h-full w-[320px] bg-surface-container-low flex-col py-lg border-r border-outline-variant z-50">
<div class="px-6 mb-8">
<h1 class="font-headline-md text-headline-md font-bold text-primary">TechFix Manager</h1>
<div class="mt-4 flex items-center gap-3">
<div class="w-10 h-10 rounded-full bg-primary-container flex items-center justify-center text-on-primary-container">
<span class="material-symbols-outlined">person</span>
</div>
<div>
<p class="font-label-lg text-on-surface">สาขาหลัก</p>
<p class="text-xs text-on-surface-variant">สิทธิ์ผู้ดูแลระบบ</p>
</div>
</div>
</div>
<nav class="flex-1 space-y-1">
<a class="flex items-center gap-3 bg-primary-container text-on-primary-container font-bold rounded-full mx-2 px-4 py-3 transition-all" href="#repairs">
<span class="material-symbols-outlined">build</span>
<span>งานซ่อม</span>
</a>
<a class="flex items-center gap-3 text-on-surface-variant px-4 py-3 mx-2 hover:bg-surface-container-high transition-all rounded-full" href="#reporting">
<span class="material-symbols-outlined">analytics</span>
<span>รายงาน</span>
</a>
<a class="flex items-center gap-3 text-on-surface-variant px-4 py-3 mx-2 hover:bg-surface-container-high transition-all rounded-full" href="#staff">
<span class="material-symbols-outlined">groups</span>
<span>พนักงาน</span>
</a>
<a class="flex items-center gap-3 text-on-surface-variant px-4 py-3 mx-2 hover:bg-surface-container-high transition-all rounded-full" href="#inventory">
<span class="material-symbols-outlined">inventory_2</span>
<span>คลังสินค้า</span>
</a>
<a class="flex items-center gap-3 text-on-surface-variant px-4 py-3 mx-2 hover:bg-surface-container-high transition-all rounded-full" href="#settings">
<span class="material-symbols-outlined">settings</span>
<span>ตั้งค่า</span>
</a>
</nav>
<div class="mt-auto px-4">
<button class="flex items-center gap-3 text-error w-full px-4 py-3 hover:bg-error-container/20 transition-all rounded-full" onclick="handleLogout()">
<span class="material-symbols-outlined">logout</span>
<span>ออกจากระบบ</span>
</button>
</div>
</aside>
<!-- Top App Bar - Mobile Header -->
<header class="fixed top-0 w-full z-50 bg-surface md:w-[calc(100%-320px)] flex items-center justify-between px-margin-mobile h-touch-target border-b border-outline-variant md:border-none pt-safe">
<div class="flex items-center gap-2">
<button class="md:hidden text-primary p-2" onclick="toggleMobileMenu()">
<span class="material-symbols-outlined">menu</span>
</button>
<span class="font-headline-md text-headline-md font-bold text-primary">TechFix Manager</span>
</div>
<div class="w-8 h-8 rounded-full bg-secondary-container flex items-center justify-center cursor-pointer" onclick="openProfile()">
<span class="material-symbols-outlined text-sm">person</span>
</div>
</header>
<!-- Main Content Canvas -->
<main class="pt-24 pb-20 px-margin-mobile md:px-margin-desktop max-w-7xl mx-auto">
<!-- Search & Filter Section -->
<section>
<div class="relative group">
<span class="absolute left-4 top-1/2 -translate-y-1/2 material-symbols-outlined text-outline">search</span>
<input class="w-full h-touch-target pl-12 pr-4 bg-surface-container rounded-xl border-none focus:ring-2 focus:ring-primary text-body-md transition-shadow" id="mainSearch" placeholder="ค้นหาด้วย IMEI หรือ ชื่อลูกค้า..." type="text">
</div>
<div class="flex gap-2 mt-4 overflow-x-auto pb-2 no-scrollbar">
<button class="status-chip bg-primary-container text-on-primary-container whitespace-nowrap active:scale-95 transition-transform" onclick="filterStatus('all')">ทั้งหมด</button>
<button class="status-chip bg-surface-container-high text-on-surface-variant whitespace-nowrap active:scale-95 transition-transform" onclick="filterStatus('pending_price')">รอแจ้งราคา</button>
<button class="status-chip bg-surface-container-high text-on-surface-variant whitespace-nowrap active:scale-95 transition-transform" onclick="filterStatus('repairing')">กำลังซ่อม</button>
<button class="status-chip bg-surface-container-high text-on-surface-variant whitespace-nowrap active:scale-95 transition-transform" onclick="filterStatus('completed')">ซ่อมเสร็จแล้ว</button>
</div>
</section>
<!-- Repairs Bento Grid / List -->
<section class="mt-lg grid grid-cols-1 lg:grid-cols-2 gap-md" id="repairsList">
<!-- Repair Card 1 -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl p-md flex flex-col gap-sm shadow-sm hover:shadow-md transition-all active:scale-[0.99]" data-status="pending_price">
<div class="flex justify-between items-start">
<div class="flex gap-3">
<div class="w-12 h-12 bg-secondary-container rounded-lg flex items-center justify-center">
<span class="material-symbols-outlined text-on-secondary-container">smartphone</span>
</div>
<div>
<h3 class="font-headline-md text-headline-md text-on-surface">สมชาย รักดี</h3>
<p class="text-sm text-on-surface-variant">iPhone 14 Pro - IMEI: 358201...942</p>
</div>
</div>
<span class="status-chip bg-tertiary-container text-on-tertiary-container">รอแจ้งราคา</span>
</div>
<div class="py-2 px-3 bg-surface-container-low rounded-lg">
<p class="text-sm font-semibold text-outline">อาการเสีย:</p>
<p class="text-body-md">หน้าจอแตก ทัชสกรีนไม่ได้บางจุด ต้องการเปลี่ยนจอแท้</p>
</div>
<div class="flex items-center justify-between mt-2 pt-2 border-t border-outline-variant">
<div class="flex gap-2">
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-surface-container hover:bg-primary-container hover:text-on-primary-container transition-colors" onclick="editRepair('1')">
<span class="material-symbols-outlined">edit</span>
</button>
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-surface-container hover:bg-error-container hover:text-on-error-container transition-colors" onclick="deleteRepair('1')">
<span class="material-symbols-outlined">delete</span>
</button>
</div>
<button class="h-touch-target px-6 bg-primary text-on-primary rounded-lg font-bold flex items-center gap-2 active:opacity-90" onclick="window.location.href='tel:0812345678'">
<span class="material-symbols-outlined text-xl">call</span>
                        โทรหาลูกค้า
                    </button>
</div>
</div>
<!-- Repair Card 2 -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl p-md flex flex-col gap-sm shadow-sm hover:shadow-md transition-all active:scale-[0.99]" data-status="repairing">
<div class="flex justify-between items-start">
<div class="flex gap-3">
<div class="w-12 h-12 bg-secondary-container rounded-lg flex items-center justify-center">
<span class="material-symbols-outlined text-on-secondary-container">laptop_mac</span>
</div>
<div>
<h3 class="font-headline-md text-headline-md text-on-surface">วิภาวรรณ สดใส</h3>
<p class="text-sm text-on-surface-variant">MacBook Air M2 - S/N: QX6G...</p>
</div>
</div>
<span class="status-chip bg-primary-container text-on-primary-container">กำลังซ่อม</span>
</div>
<div class="py-2 px-3 bg-surface-container-low rounded-lg">
<p class="text-sm font-semibold text-outline">อาการเสีย:</p>
<p class="text-body-md">เปิดไม่ติด ชาร์จไฟไม่เข้า คาดว่าบอร์ดมีปัญหา</p>
</div>
<div class="flex items-center justify-between mt-2 pt-2 border-t border-outline-variant">
<div class="flex gap-2">
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-surface-container" onclick="editRepair('2')">
<span class="material-symbols-outlined">edit</span>
</button>
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-surface-container" onclick="deleteRepair('2')">
<span class="material-symbols-outlined">delete</span>
</button>
</div>
<button class="h-touch-target px-6 bg-primary text-on-primary rounded-lg font-bold flex items-center gap-2" onclick="viewHistory('2')">
<span class="material-symbols-outlined">history</span>
                        ประวัติซ่อม
                    </button>
</div>
</div>
<!-- Repair Card 3 (Completed) -->
<div class="bg-surface-container-lowest border-2 border-primary rounded-xl p-md flex flex-col gap-sm shadow-md transition-all active:scale-[0.99]" data-status="completed">
<div class="flex justify-between items-start">
<div class="flex gap-3">
<div class="w-12 h-12 bg-secondary-container rounded-lg flex items-center justify-center">
<span class="material-symbols-outlined text-on-secondary-container">tablet_android</span>
</div>
<div>
<h3 class="font-headline-md text-headline-md text-on-surface">นพดล ขยันงาน</h3>
<p class="text-sm text-on-surface-variant">iPad Pro 11" - IMEI: 99122...</p>
</div>
</div>
<span class="status-chip bg-green-600 text-white">ซ่อมเสร็จแล้ว</span>
</div>
<div class="py-2 px-3 bg-green-50 rounded-lg border border-green-100">
<div class="flex items-center justify-between">
<span class="text-sm font-semibold text-green-700">แจ้งเตือน:</span>
<span class="text-xs text-green-600">พร้อมส่งคืน</span>
</div>
<p class="text-body-md text-green-900">เปลี่ยนแบตเตอรี่เรียบร้อย ทดสอบผ่านทุกขั้นตอน</p>
</div>
<div class="flex items-center justify-between mt-2 pt-2 border-t border-outline-variant">
<div class="flex gap-2">
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-surface-container" onclick="editRepair('3')">
<span class="material-symbols-outlined">edit</span>
</button>
</div>
<button class="h-touch-target px-6 bg-green-600 text-white rounded-lg font-bold flex items-center gap-2" onclick="returnToCustomer('3')">
<span class="material-symbols-outlined">check_circle</span>
                        ส่งคืนลูกค้า
                    </button>
</div>
</div>
<!-- Repair Card 4 (Claiming) -->
<div class="bg-surface-container-lowest border border-outline-variant rounded-xl p-md flex flex-col gap-sm transition-all" data-status="claiming">
<div class="flex justify-between items-start">
<div class="flex gap-3">
<div class="w-12 h-12 bg-secondary-container rounded-lg flex items-center justify-center">
<span class="material-symbols-outlined text-on-secondary-container">watch</span>
</div>
<div>
<h3 class="font-headline-md text-headline-md text-on-surface">ขวัญชัย ใจดี</h3>
<p class="text-sm text-on-surface-variant">Apple Watch S8 - IMEI: 2210...</p>
</div>
</div>
<span class="status-chip bg-error-container text-on-error-container">กำลังเคลม</span>
</div>
<div class="py-2 px-3 bg-surface-container-low rounded-lg">
<p class="text-sm font-semibold text-outline">สถานะเคลม:</p>
<p class="text-body-md">ส่งศูนย์ iCare เช็คโมดูลหน้าจอ รอบริษัทตอบกลับ</p>
</div>
<div class="flex items-center justify-between mt-2 pt-2 border-t border-outline-variant">
<div class="flex gap-2">
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-surface-container" onclick="editRepair('4')">
<span class="material-symbols-outlined">edit</span>
</button>
</div>
<button class="h-touch-target px-6 bg-secondary text-on-secondary rounded-lg font-bold flex items-center gap-2" onclick="viewDetails('4')">
<span class="material-symbols-outlined">info</span>
                        ดูรายละเอียด
                    </button>
</div>
</div>
</section>
<!-- Quick Status Update Panel -->
<div class="mt-xl p-lg bg-surface-container-highest rounded-2xl border-2 border-dashed border-outline-variant">
<h2 class="font-headline-lg text-headline-lg text-primary mb-lg">อัปเดตสถานะด่วน</h2>
<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-sm">
<button class="flex flex-col items-center justify-center gap-2 h-24 bg-surface-container-lowest border border-outline-variant rounded-xl hover:bg-tertiary-container hover:text-on-tertiary-container transition-all active:scale-95" onclick="updateStatusQuickly('pending_price')">
<span class="material-symbols-outlined text-3xl">pending_actions</span>
<span class="text-xs font-bold">รอแจ้งราคา</span>
</button>
<button class="flex flex-col items-center justify-center gap-2 h-24 bg-surface-container-lowest border border-outline-variant rounded-xl hover:bg-primary-container hover:text-on-primary-container transition-all active:scale-95" onclick="updateStatusQuickly('repairing')">
<span class="material-symbols-outlined text-3xl">construction</span>
<span class="text-xs font-bold">กำลังซ่อม</span>
</button>
<button class="flex flex-col items-center justify-center gap-2 h-24 bg-surface-container-lowest border border-outline-variant rounded-xl hover:bg-error-container hover:text-on-error-container transition-all active:scale-95" onclick="updateStatusQuickly('claiming')">
<span class="material-symbols-outlined text-3xl">assignment_return</span>
<span class="text-xs font-bold">กำลังเคลม</span>
</button>
<button class="flex flex-col items-center justify-center gap-2 h-24 bg-green-100 border border-green-200 text-green-800 rounded-xl hover:bg-green-600 hover:text-white transition-all active:scale-95" onclick="updateStatusQuickly('completed')">
<span class="material-symbols-outlined text-3xl">check_circle</span>
<span class="text-xs font-bold">ซ่อมเสร็จแล้ว</span>
</button>
<button class="flex flex-col items-center justify-center gap-2 h-24 bg-surface-container-lowest border border-outline-variant rounded-xl hover:bg-green-container hover:text-on-green-container transition-all active:scale-95" onclick="updateStatusQuickly('claimed')">
<span class="material-symbols-outlined text-3xl">verified</span>
<span class="text-xs font-bold">ซ่อมเสร็จเคลม</span>
</button>
<button class="flex flex-col items-center justify-center gap-2 h-24 bg-surface-container-lowest border border-outline-variant rounded-xl hover:bg-outline-variant transition-all active:scale-95" onclick="updateStatusQuickly('returned')">
<span class="material-symbols-outlined text-3xl">keyboard_return</span>
<span class="text-xs font-bold">ส่งคืนแล้ว</span>
</button>
</div>
</div>
</main>
<!-- Bottom Navigation Bar - Mobile Only -->
<nav class="md:hidden fixed bottom-0 w-full z-50 h-[80px] bg-surface flex justify-around items-center border-t border-outline-variant pb-safe">
<a class="flex flex-col items-center justify-center text-on-surface-variant flex-1 h-full" href="#dashboard">
<span class="material-symbols-outlined">dashboard</span>
<span class="font-label-sm text-label-sm">หน้าแรก</span>
</a>
<a class="flex flex-col items-center justify-center bg-secondary-container text-on-secondary-container rounded-xl px-4 py-1 mx-2" href="#repairs">
<span class="material-symbols-outlined">build</span>
<span class="font-label-sm text-label-sm">งานซ่อม</span>
</a>
<button class="flex flex-col items-center justify-center text-on-surface-variant flex-1 h-full" onclick="createNewEntry()">
<span class="material-symbols-outlined">add_circle</span>
<span class="font-label-sm text-label-sm">เพิ่มงานใหม่</span>
</button>
<a class="flex flex-col items-center justify-center text-on-surface-variant flex-1 h-full" href="#inventory">
<span class="material-symbols-outlined">inventory_2</span>
<span class="font-label-sm text-label-sm">คลังสินค้า</span>
</a>
</nav>
<!-- Floating Action Button -->
<button class="fixed right-6 bottom-24 md:bottom-10 bg-primary text-on-primary w-14 h-14 rounded-full shadow-lg flex items-center justify-center z-40 active:scale-90 transition-all hover:bg-primary-container" onclick="createNewEntry()">
<span class="material-symbols-outlined text-3xl">add</span>
</button>
<script>
        // Internal Navigation & Interaction Logic
        function handleLogout() {
            if(confirm('คุณแน่ใจหรือไม่ว่าต้องการออกจากระบบ?')) {
                console.log('Logging out...');
            }
        }

        function toggleMobileMenu() {
            console.log('Menu toggled');
            // Logic for mobile drawer can be added here
        }

        function createNewEntry() {
            console.log('Opening new entry form...');
        }

        function editRepair(id) {
            console.log('Editing repair:', id);
        }

        function deleteRepair(id) {
            if(confirm('ยืนยันการลบข้อมูลงานซ่อมนี้?')) {
                console.log('Deleting repair:', id);
            }
        }

        function filterStatus(status) {
            const cards = document.querySelectorAll('#repairsList > div');
            cards.forEach(card => {
                if (status === 'all' || card.dataset.status === status) {
                    card.style.display = 'flex';
                } else {
                    card.style.display = 'none';
                }
            });
            // Update chip styles
            document.querySelectorAll('.status-chip').forEach(chip => {
                chip.classList.remove('bg-primary-container', 'text-on-primary-container');
                chip.classList.add('bg-surface-container-high', 'text-on-surface-variant');
            });
            event.currentTarget.classList.remove('bg-surface-container-high', 'text-on-surface-variant');
            event.currentTarget.classList.add('bg-primary-container', 'text-on-primary-container');
        }

        function updateStatusQuickly(status) {
            console.log('Updating status to:', status);
        }

        // Search logic
        const searchInput = document.getElementById('mainSearch');
        searchInput.addEventListener('input', (e) => {
            const query = e.target.value.toLowerCase();
            const cards = document.querySelectorAll('#repairsList > div');
            
            cards.forEach(card => {
                const text = card.textContent.toLowerCase();
                if (text.includes(query)) {
                    card.style.display = 'flex';
                } else {
                    card.style.display = 'none';
                }
            });
        });

        // Other generic handlers
        function viewHistory(id) { console.log('Viewing history:', id); }
        function returnToCustomer(id) { console.log('Returning to customer:', id); }
        function viewDetails(id) { console.log('Viewing details:', id); }
        function openProfile() { console.log('Opening profile...'); }
    </script>
</body></html>
