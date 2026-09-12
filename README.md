<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rafi Store - Top Up Game Terpercaya & Termurah</title>
    <style>
        :root {
            --primary-color: #4f46e5;
            --primary-dark: #4338ca;
            --primary-light: #6366f1;
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --accent-price: #38bdf8;
            --badge-bg: #312e81;
            --badge-text: #818cf8;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Navbar & Cart Icon */
        nav {
            background-color: rgba(30, 41, 59, 0.9);
            backdrop-filter: blur(10px);
            padding: 15px 30px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid #334155;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 800;
            color: var(--accent-price);
            letter-spacing: -0.5px;
        }

        .nav-actions {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .search-box {
            padding: 8px 15px;
            border-radius: 20px;
            border: 1px solid #475569;
            background-color: #0f172a;
            color: white;
            outline: none;
            font-size: 0.9rem;
            width: 220px;
            transition: all 0.3s;
        }

        .search-box:focus {
            border-color: var(--accent-price);
            width: 260px;
            box-shadow: 0 0 0 3px rgba(56, 189, 248, 0.2);
        }

        .cart-btn {
            background-color: #334155;
            border: 1px solid #475569;
            padding: 10px 18px;
            border-radius: 20px;
            cursor: pointer;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: all 0.2s;
            color: var(--text-main);
        }

        .cart-btn:hover {
            background-color: #475569;
            transform: translateY(-1px);
        }

        .cart-badge {
            background-color: var(--accent-price);
            color: #0f172a;
            border-radius: 50%;
            padding: 2px 7px;
            font-size: 0.75rem;
            font-weight: 700;
        }

        /* Header & Banner Styles */
        header {
            background: linear-gradient(135deg, #312e81, #1e1b4b, #0f172a);
            color: white;
            padding: 60px 20px;
            text-align: center;
            border-bottom: 1px solid #334155;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 12px;
            font-weight: 800;
            letter-spacing: -0.5px;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.85;
            max-width: 650px;
            margin: 0 auto;
            font-weight: 300;
        }

        /* Main Container */
        .container {
            max-width: 1100px;
            margin: 40px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        /* Product Card Styles */
        .card {
            background: var(--card-bg);
            border-radius: 16px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            overflow: hidden;
            display: flex;
            flex-direction: column;
            transition: all 0.3s cubic-bezier(0.165, 0.84, 0.44, 1);
            border: 1px solid #334155;
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 35px rgba(0,0,0,0.4);
            border-color: var(--primary-light);
        }

        .card-img-wrapper {
            width: 100%;
            height: 180px;
            overflow: hidden;
            background-color: #0f172a;
            position: relative;
        }

        .card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.6s ease;
        }

        .card:hover img {
            transform: scale(1.08);
        }

        .card-content {
            padding: 24px;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .card h3 {
            font-size: 1.25rem;
            margin-bottom: 10px;
            color: var(--text-main);
            font-weight: 700;
        }

        .description {
            font-size: 0.92rem;
            color: var(--text-muted);
            margin-bottom: 15px;
            line-height: 1.5;
        }

        .input-group {
            margin-bottom: 15px;
        }

        .input-group label {
            font-size: 0.8rem;
            color: var(--text-muted);
            display: block;
            margin-bottom: 5px;
        }

        .input-group input, .input-group select {
            width: 100%;
            padding: 8px 12px;
            background: #0f172a;
            border: 1px solid #475569;
            border-radius: 8px;
            color: white;
            font-size: 0.9rem;
            outline: none;
        }

        .input-group input:focus, .input-group select:focus {
            border-color: var(--accent-price);
        }

        .price-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .card .price {
            color: var(--accent-price);
            font-weight: 800;
            font-size: 1.15rem;
        }

        .badge {
            background-color: var(--badge-bg);
            color: var(--badge-text);
            font-size: 0.75rem;
            padding: 5px 10px;
            border-radius: 20px;
            font-weight: 700;
        }

        .btn-add {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 12px 15px;
            border-radius: 10px;
            cursor: pointer;
            font-size: 0.95rem;
            font-weight: 700;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            transition: all 0.2s ease;
        }

        .btn-add:hover {
            background-color: var(--primary-light);
            box-shadow: 0 4px 12px rgba(79, 70, 229, 0.4);
        }

        /* Toast Notification */
        .toast {
            position: fixed;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%) translateY(100px);
            background-color: #334155;
            color: white;
            padding: 12px 24px;
            border-radius: 30px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
            font-weight: 600;
            font-size: 0.9rem;
            z-index: 2000;
            opacity: 0;
            transition: all 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
            border: 1px solid #475569;
        }

        .toast.show {
            transform: translateX(-50%) translateY(0);
            opacity: 1;
        }

        /* Cart Modal Drawer */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.7);
            backdrop-filter: blur(4px);
            display: none;
            justify-content: flex-end;
            z-index: 1000;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .modal-overlay.active {
            display: flex;
            opacity: 1;
        }

        .cart-drawer {
            background: #1e293b;
            width: 100%;
            max-width: 420px;
            height: 100%;
            padding: 30px;
            display: flex;
            flex-direction: column;
            box-shadow: -10px 0 30px rgba(0,0,0,0.5);
            transform: translateX(100%);
            transition: transform 0.3s cubic-bezier(0.16, 1, 0.3, 1);
            border-left: 1px solid #334155;
        }

        .modal-overlay.active .cart-drawer {
            transform: translateX(0);
        }

        .cart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #334155;
            padding-bottom: 20px;
        }

        .cart-header h3 {
            font-size: 1.3rem;
            font-weight: 700;
        }

        .close-cart {
            background: #334155;
            border: none;
            width: 36px;
            height: 36px;
            border-radius: 50%;
            font-size: 1.2rem;
            cursor: pointer;
            color: #f8fafc;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: background 0.2s;
        }

        .close-cart:hover {
            background: #475569;
        }

        .cart-items {
            flex-grow: 1;
            overflow-y: auto;
            padding: 20px 0;
        }

        .cart-item {
            background: #0f172a;
            padding: 12px;
            border-radius: 10px;
            margin-bottom: 12px;
            border: 1px solid #334155;
        }

        .cart-item-info h4 {
            font-size: 0.95rem;
            margin-bottom: 2px;
            font-weight: 600;
        }

        .cart-item-info p {
            font-size: 0.8rem;
            color: var(--text-muted);
            margin-bottom: 6px;
        }

        .cart-item-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .cart-item-row span {
            font-size: 0.9rem;
            color: var(--accent-price);
            font-weight: 700;
        }

        .btn-delete {
            background: #ef4444;
            color: white;
            border: none;
            padding: 4px 10px;
            border-radius: 6px;
            cursor: pointer;
            font-size: 0.75rem;
            font-weight: 600;
        }

        .btn-delete:hover {
            background: #dc2626;
        }

        .cart-footer {
            border-top: 1px solid #334155;
            padding-top: 20px;
        }

        .cart-total {
            display: flex;
            justify-content: space-between;
            font-size: 1.15rem;
            font-weight: 700;
            margin-bottom: 20px;
        }

        .btn-checkout {
            background-color: #25d366;
            color: white;
            border: none;
            padding: 14px;
            border-radius: 12px;
            width: 100%;
            font-size: 1rem;
            font-weight: 700;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.3);
        }

        .btn-checkout:hover {
            background-color: #1ebe57;
            transform: translateY(-2px);
        }

        .empty-cart {
            text-align: center;
            color: var(--text-muted);
            margin-top: 60px;
            font-size: 0.95rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 30px;
            background-color: #1e293b;
            color: var(--text-muted);
            font-size: 0.9rem;
            border-top: 1px solid #334155;
            margin-top: 60px;
        }

        @media(max-width: 600px) {
            .search-box {
                display: none;
            }
            header h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Navbar -->
    <nav>
        <div class="logo">🎮 StoreKu Games</div>
        <div class="nav-actions">
            <input type="text" class="search-box" id="searchBox" placeholder="Cari game..." onkeyup="filterProduk()">
            <button class="cart-btn" onclick="toggleCart()">
                🛒 Keranjang <span class="cart-badge" id="cartCount">0</span>
            </button>
        </div>
    </nav>

    <header>
        <h1>Top Up Game Instan & Aman</h1>
        <p>Pilih game favoritmu, masukkan data akun, dan selesaikan transaksi dengan cepat via WhatsApp.</p>
    </header>

    <!-- Daftar Game / Produk -->
    <div class="container" id="productContainer">
        
        <!-- Game 1: Mobile Legends -->
        <div class="card" data-name="Mobile Legends">
            <div class="card-img-wrapper">
                <img src="https://images.unsplash.com/photo-1542751371-adc38448a05e?auto=format&fit=crop&w=500&q=80" alt="Mobile Legends">
            </div>
            <div class="card-content">
                <h3>Mobile Legends</h3>
                <p class="description">Diamond Resmi & Legal 100% Instant Masuk.</p>
                <div class="input-group">
                    <label>ID Game & Server</label>
                    <input type="text" id="id-ml" placeholder="Contoh: 12345678 (1234)">
                </div>
                <div class="input-group">
                    <label>Nominal Item</label>
                    <select id="item-ml">
                        <option value="86 Diamond|20000">86 Diamonds - Rp 20.000</option>
                        <option value="172 Diamond|40000">172 Diamonds - Rp 40.000</option>
                        <option value="257 Diamond|60000">257 Diamonds - Rp 60.000</option>
                        <option value="Starlight Member|145000">Starlight Member - Rp 145.000</option>
                    </select>
                </div>
                <div class="price-row">
                    <span class="price" id="price-ml">Rp 20.000</span>
                    <span class="badge">Instant</span>
                </div>
                <button class="btn-add" onclick="tambahKeKeranjang('Mobile Legends', 'id-ml', 'item-ml')">
                    + Tambah ke Keranjang
                </button>
            </div>
        </div>

        <!-- Game 2: Free Fire -->
        <div class="card" data-name="Free Fire">
            <div class="card-img-wrapper">
                <img src="https://images.unsplash.com/photo-1538481199705-c710c4e965fc?auto=format&fit=crop&w=500&q=80" alt="Free Fire">
            </div>
            <div class="card-content">
                <h3>Free Fire</h3>
                <p class="description">Top up Diamond FF aman, murah, dan terpercaya.</p>
                <div class="input-group">
                    <label>ID Player (User ID)</label>
                    <input type="text" id="id-ff" placeholder="Contoh: 123456789">
                </div>
                <div class="input-group">
                    <label>Nominal Item</label>
                    <select id="item-ff">
                        <option value="140 Diamond|20000">140 Diamonds - Rp 20.000</option>
                        <option value="355 Diamond|50000">355 Diamonds - Rp 50.000</option>
                        <option value="720 Diamond|100000">720 Diamonds - Rp 100.000</option>
                    </select>
                </div>
                <div class="price-row">
                    <span class="price" id="price-ff">Rp 20.000</span>
                    <span class="badge">Hot Promo</span>
                </div>
                <button class="btn-add" onclick="tambahKeKeranjang('Free Fire', 'id-ff', 'item-ff')">
                    + Tambah ke Keranjang
                </button>
            </div>
        </div>

        <!-- Game 3: PUBG Mobile -->
        <div class="card" data-name="PUBG Mobile">
            <div class="card-img-wrapper">
                <img src="https://images.unsplash.com/photo-1511512578047-dfb367046420?auto=format&fit=crop&w=500&q=80" alt="PUBG Mobile">
            </div>
            <div class="card-content">
                <h3>PUBG Mobile</h3>
                <p class="description">Official UC Purchase aman anti-minus.</p>
                <div class="input-group">
                    <label>Character ID</label>
                    <input type="text" id="id-pubg" placeholder="Contoh: 5123456789">
                </div>
                <div class="input-group">
                    <label>Nominal Item</label>
                    <select id="item-pubg">
                        <option value="60 UC|15000">60 UC - Rp 15.000</option>
                        <option value="325 UC|75000">325 UC - Rp 75.000</option>
                        <option value="660 UC|150000">660 UC - Rp 150.000</option>
                    </select>
                </div>
                <div class="price-row">
                    <span class="price" id="price-pubg">Rp 15.000</span>
                    <span class="badge">Terlaris</span>
                </div>
                <button class="btn-add" onclick="tambahKeKeranjang('PUBG Mobile', 'id-pubg', 'item-pubg')">
                    + Tambah ke Keranjang
                </button>
            </div>
        </div>

    </div>

    <!-- Toast Notification -->
    <div class="toast" id="toastNotification">Pesanan ditambahkan ke keranjang!</div>

    <!-- Modal / Drawer Keranjang -->
    <div class="modal-overlay" id="cartModal" onclick="outsideClick(event)">
        <div class="cart-drawer">
            <div class="cart-header">
                <h3>Keranjang Top Up</h3>
                <button class="close-cart" onclick="toggleCart()">&times;</button>
            </div>
            
            <div class="cart-items" id="cartItemsContainer">
                <p class="empty-cart">Keranjang masih kosong</p>
            </div>

            <div class="cart-footer">
                <div class="cart-total">
                    <span>Total:</span>
                    <span id="cartTotalPrice">Rp 0</span>
                </div>
                <button class="btn-checkout" onclick="checkoutWhatsApp()">
                    💬 Checkout via WhatsApp
                </button>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2026 StoreKu Games. All rights reserved.</p>
    </footer>

    <script>
        let keranjang = [];

        document.getElementById('item-ml').addEventListener('change', function() {
            let harga = parseInt(this.value.split('|')[1]);
            document.getElementById('price-ml').innerText = 'Rp ' + harga.toLocaleString('id-ID');
        });
        document.getElementById('item-ff').addEventListener('change', function() {
            let harga = parseInt(this.value.split('|')[1]);
            document.getElementById('price-ff').innerText = 'Rp ' + harga.toLocaleString('id-ID');
        });
        document.getElementById('item-pubg').addEventListener('change', function() {
            let harga = parseInt(this.value.split('|')[1]);
            document.getElementById('price-pubg').innerText = 'Rp ' + harga.toLocaleString('id-ID');
        });

        function toggleCart() {
            const modal = document.getElementById('cartModal');
            if (modal.classList.contains('active')) {
                modal.classList.remove('active');
                setTimeout(() => modal.style.display = 'none', 300);
            } else {
                modal.style.display = 'flex';
                setTimeout(() => modal.classList.add('active'), 10);
            }
        }

        function outsideClick(event) {
            const modal = document.getElementById('cartModal');
            if (event.target === modal) {
                toggleCart();
            }
        }

        function showToast(message) {
            const toast = document.getElementById('toastNotification');
            toast.innerText = message;
            toast.classList.add('show');
            setTimeout(() => {
                toast.classList.remove('show');
            }, 2500);
        }

        function tambahKeKeranjang(namaGame, idInputId, selectId) {
            let userId = document.getElementById(idInputId).value.trim();
            let selectElement = document.getElementById(selectId);
            let selectedValue = selectElement.value.split('|');
            let itemName = selectedValue[0];
            let itemHarga = parseInt(selectedValue[1]);

            if (!userId) {
                showToast('⚠️ Masukkan ID Akun Game terlebih dahulu!');
                return;
            }

            keranjang.push({
                game: namaGame,
                userId: userId,
                item: itemName,
                harga: itemHarga
            });

            document.getElementById(idInputId).value = '';
            updateTampilanKeranjang();
            showToast(`${namaGame} (${itemName}) masuk keranjang! 🎮`);
        }

        function hapusItem(index) {
            keranjang.splice(index, 1);
            updateTampilanKeranjang();
        }

        function updateTampilanKeranjang() {
            const container = document.getElementById('cartItemsContainer');
            const countBadge = document.getElementById('cartCount');
            const totalPriceElement = document.getElementById('cartTotalPrice');

            container.innerHTML = '';
            let totalPrice = 0;

            if (keranjang.length === 0) {
                container.innerHTML = '<p class="empty-cart">Keranjang masih kosong</p>';
                countBadge.innerText = '0';
                totalPriceElement.innerText = 'Rp 0';
                return;
            }

            keranjang.forEach((pesanan, index) => {
                totalPrice += pesanan.harga;

                container.innerHTML += `
                    <div class="cart-item">
                        <div class="cart-item-info">
                            <h4>${pesanan.game} - ${pesanan.item}</h4>
                            <p>ID: <b>${pesanan.userId}</b></p>
                        </div>
                        <div class="cart-item-row">
                            <span>Rp ${pesanan.harga.toLocaleString('id-ID')}</span>
                            <button class="btn-delete" onclick="hapusItem(${index})">Hapus</button>
                        </div>
                    </div>
                `;
            });

            countBadge.innerText = keranjang.length;
            totalPriceElement.innerText = `Rp ${totalPrice.toLocaleString('id-ID')}`;
        }

        function filterProduk() {
            let keyword = document.getElementById('searchBox').value.toLowerCase();
            let cards = document.querySelectorAll('.card');

            cards.forEach(card => {
                let name = card.getAttribute('data-name').toLowerCase();
                if (name.includes(keyword)) {
                    card.style.display = 'flex';
                } else {
                    card.style.display = 'none';
                }
            });
        }

        function checkoutWhatsApp() {
            if (keranjang.length === 0) {
                showToast('Keranjang Anda masih kosong!');
                return;
            }

            const nomorTujuan = "6287794194585";
            let pesan = "Halo Admin StoreKu Games, saya ingin melakukan top up pesanan berikut:\n\n";

            let totalKeseluruhan = 0;
            keranjang.forEach((pesanan, index) => {
                totalKeseluruhan += pesanan.harga;
                pesan += `${index + 1}. *${pesanan.game}*\n`;
                pesan += `   - Item: ${pesanan.item}\n`;
                pesan += `   - ID Akun: ${pesanan.userId}\n`;
                pesan += `   - Harga: Rp ${pesanan.harga.toLocaleString('id-ID')}\n\n`;
            });

            pesan += `*Total Pembayaran: Rp ${totalKeseluruhan.toLocaleString('id-ID')}*`;
            pesan += "\n\nMohon info QRIS / nomor rekening untuk pembayarannya ya. Terima kasih!";

            const urlWA = `https://wa.me/${nomorTujuan}?text=${encodeURIComponent(pesan)}`;
            window.open(urlWA, '_blank');
        }
    </script>
</body>
</html>
