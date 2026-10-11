<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Delta Premium Hub | مركز السكريبتات الأسطوري</title>
    <!-- استدعاء خط Cairo -->
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700;900&display=swap" rel="stylesheet">
    <!-- استدعاء Firebase -->
    <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-app-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-database-compat.js"></script>
    
    <style>
        * { box-sizing: border-box; }
        body { 
            background: linear-gradient(135deg, #0d0f18 0%, #05070a 100%); 
            color: #ffffff; 
            font-family: 'Cairo', sans-serif; 
            text-align: center; 
            padding: 20px; 
            min-height: 100vh;
            margin: 0;
        }
        
        .container { max-width: 500px; margin: 0 auto; }

        .glass-box { 
            background: rgba(25, 30, 45, 0.75); 
            backdrop-filter: blur(14px);
            border: 1px solid rgba(0, 255, 204, 0.25); 
            border-radius: 16px; 
            padding: 25px; 
            margin: 20px auto; 
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.6); 
        }

        h1 { font-weight: 900; color: #00ffcc; text-shadow: 0 0 20px rgba(0,255,204,0.4); font-size: 26px; margin-bottom: 5px; }
        h2 { font-size: 20px; color: #fff; margin-bottom: 15px; }
        
        input, textarea { 
            width: 100%; 
            padding: 12px 15px; 
            margin: 10px 0; 
            background: rgba(10, 12, 18, 0.85); 
            border: 1px solid rgba(255, 255, 255, 0.15); 
            color: #00ffcc; 
            border-radius: 10px; 
            font-size: 15px; 
            outline: none;
            transition: all 0.3s;
        }
        input:focus, textarea:focus { border-color: #00ffcc; box-shadow: 0 0 12px rgba(0,255,204,0.4); }

        .btn-neon { 
            background: linear-gradient(135deg, #00ffcc 0%, #00b894 100%); 
            color: #05070a; 
            border: none; 
            padding: 12px 20px; 
            font-weight: 900; 
            border-radius: 10px; 
            cursor: pointer; 
            width: 100%; 
            margin-top: 10px;
            font-size: 16px;
            box-shadow: 0 4px 15px rgba(0,255,204,0.4);
            transition: transform 0.2s, box-shadow 0.2s;
        }
        .btn-neon:active { transform: scale(0.98); }
        .btn-neon:hover { box-shadow: 0 6px 20px rgba(0,255,204,0.7); }

        .btn-danger { 
            background: linear-gradient(135deg, #ff4d4d 0%, #c0392b 100%); 
            color: #fff; 
            box-shadow: 0 4px 15px rgba(255,77,77,0.4);
        }

        .error { color: #ff5252; font-size: 13px; margin: 5px 0; font-weight: bold; }
        .success { color: #00ffcc; font-size: 13px; margin: 5px 0; font-weight: bold; }
        .hidden { display: none; }

        .code-box { 
            background: #090b10; 
            border: 1px dashed rgba(0,255,204,0.3);
            padding: 12px; 
            border-radius: 8px; 
            font-family: monospace; 
            font-size: 12px; 
            color: #00ffaa; 
            word-break: break-all; 
            margin: 12px 0; 
            text-align: left; 
            direction: ltr;
            max-height: 100px;
            overflow-y: auto;
        }

        .script-card { text-align: right; position: relative; overflow: hidden; }
        .script-card::before {
            content: '';
            position: absolute;
            top: 0; right: 0; width: 4px; height: 100%;
            background: #00ffcc;
        }

        .badge {
            background: rgba(0,255,204,0.1);
            color: #00ffcc;
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 11px;
            border: 1px solid rgba(0,255,204,0.3);
            display: inline-block;
            margin-bottom: 8px;
        }

        .toggle-link { margin-top: 15px; font-size: 14px; cursor: pointer; color: #00ffcc; text-decoration: underline; }
        
        .tabs { display: flex; gap: 10px; margin-bottom: 20px; }
        .tab-btn { flex: 1; padding: 10px; background: rgba(255,255,255,0.05); border: 1px solid rgba(255,255,255,0.1); color: #fff; border-radius: 8px; cursor: pointer; font-weight: bold; }
        .tab-btn.active { background: #00ffcc; color: #000; border-color: #00ffcc; }
    </style>
</head>
<body>

    <div class="container">

        <!-- تسجيل الدخول / إنشاء حساب -->
        <div id="auth-section" class="glass-box">
            <h1 id="form-title">إنشاء حساب جديد</h1>
            <p style="color: #aaa; font-size: 13px; margin-bottom: 20px;">سجل دخلك للتحكم في سكريبتاتك ونشرها</p>
            <div id="message"></div>
            
            <input type="text" id="username" placeholder="اسم المستخدم (حروف، أرقام، _ فقط)">
            <input type="password" id="password" placeholder="كلمة المرور">
            
            <button id="action-btn" class="btn-neon" onclick="handleAuth()">إنشاء الحساب</button>
            <div class="toggle-link" onclick="toggleMode()">
                <span id="toggle-text">لديك حساب بالفعل؟ تسجيل الدخول</span>
            </div>
        </div>

        <!-- الواجهة الرئيسية للموقع -->
        <div id="app-section" class="hidden">
            <div class="glass-box" style="padding: 15px; display: flex; justify-content: space-between; align-items: center;">
                <div style="text-align: right;">
                    <span style="font-size: 11px; color: #aaa;">الحساب الحالي:</span>
                    <h3 id="user-display" style="margin: 0; color: #00ffcc; font-size: 17px;"></h3>
                </div>
                <button onclick="logout()" class="btn-neon btn-danger" style="width: auto; padding: 6px 15px; font-size: 12px; margin: 0;">تسجيل الخروج 🚪</button>
            </div>

            <!-- إضافة سكريبت جديد -->
            <div class="glass-box">
                <h2>⚡ نشر سكريبت جديد لـ Delta</h2>
                <input type="text" id="script-title" placeholder="اسم اللعبة أو الميزة (مثلاً: Blox Fruits)">
                <textarea id="script-code" placeholder="loadstring(game:HttpGet('...'))()" rows="3"></textarea>
                <button class="btn-neon" onclick="uploadScript()">نشر السكريبت للجميع 🚀</button>
            </div>

            <!-- التبويب بين عرض الكل أو سكريبتاتي -->
            <div class="tabs">
                <button class="tab-btn active" id="btn-all" onclick="switchTab('all')">🌐 كل السكريبتات</button>
                <button class="tab-btn" id="btn-my" onclick="switchTab('my')">👤 سكريبتاتي والتحكم بها</button>
            </div>

            <!-- قائمة عرض السكريبتات -->
            <div id="scripts-container">
                <p style="color: #aaa;">جاري جلب البيانات السحابية...</p>
            </div>
        </div>

    </div>

    <script>
        const firebaseConfig = {
            databaseURL: "https://delta-scripts-hub-default-rtdb.firebaseio.com/"
        };
        firebase.initializeApp(firebaseConfig);
        const db = firebase.database();

        let isLoginMode = false;
        let currentView = 'all';
        let allScriptsData = {};

        function toggleMode() {
            isLoginMode = !isLoginMode;
            document.getElementById('form-title').innerText = isLoginMode ? "تسجيل الدخول" : "إنشاء حساب جديد";
            document.getElementById('action-btn').innerText = isLoginMode ? "تسجيل الدخول" : "إنشاء الحساب";
            document.getElementById('toggle-text').innerText = isLoginMode ? "ليس لديك حساب؟ إنشاء حساب جديد" : "لديك حساب بالفعل؟ تسجيل الدخول";
            document.getElementById('message').innerText = "";
        }

        function handleAuth() {
            let user = document.getElementById('username').value.trim();
            let pass = document.getElementById('password').value.trim();
            let msgBox = document.getElementById('message');

            if (!user || !pass) {
                msgBox.className = "error";
                msgBox.innerText = "❌ يرجى ملء جميع الحقول المطلوبة!";
                return;
            }

            let regex = /^[a-zA-Z0-9_]+$/;
            if (!regex.test(user)) {
                msgBox.className = "error";
                msgBox.innerText = "❌ اسم المستخدم يسمح فقط بالحروف الإنجليزية، الأرقام، و (_) بدون مسافات.";
                return;
            }

            db.ref('users/' + user).once('value').then((snapshot) => {
                let existingPass = snapshot.val();

                if (!isLoginMode) {
                    if (existingPass) {
                        msgBox.className = "error";
                        msgBox.innerText = "❌ اسم المستخدم هذا مأخوذ بالفعل، اختر اسماً آخر!";
                        return;
                    }
                    db.ref('users/' + user).set(pass);
                    msgBox.className = "success";
                    msgBox.innerText = "✅ تم إنشاء الحساب بنجاح!";
                    setTimeout(() => loginSuccess(user), 800);
                } else {
                    if (!existingPass || existingPass !== pass) {
                        msgBox.className = "error";
                        msgBox.innerText = "❌ اسم المستخدم أو كلمة المرور غير صحيحة!";
                        return;
                    }
                    loginSuccess(user);
                }
            });
        }

        function loginSuccess(user) {
            localStorage.setItem('delta_active_user', user);
            document.getElementById('auth-section').classList.add('hidden');
            document.getElementById('app-section').classList.remove('hidden');
            document.getElementById('user-display').innerText = user;
            listenToScripts();
        }

        function logout() {
            localStorage.removeItem('delta_active_user');
            location.reload();
        }

        function uploadScript() {
            let title = document.getElementById('script-title').value.trim();
            let code = document.getElementById('script-code').value.trim();
            let user = localStorage.getItem('delta_active_user');

            if (!title || !code) {
                alert("⚠️ أدخل اسم السكريبت وكود الـ Loadstring أولاً!");
                return;
            }

            let newScriptRef = db.ref('scripts').push();
            newScriptRef.set({
                title: title,
                code: code,
                author: user,
                time: new Date().toLocaleDateString()
            }, (error) => {
                if (!error) {
                    alert("🚀 تم نشر السكريبت بنجاح وأصبح محفوظاً ومتاحاً!");
                    document.getElementById('script-title').value = '';
                    document.getElementById('script-code').value = '';
                }
            });
        }

        // خاصية التحكم بالحذف 🗑️
        function deleteScript(key) {
            if (confirm("هل أنت تأكد أنك تريد حذف هذا السكريبت نهائياً؟")) {
                db.ref('scripts/' + key).remove().then(() => {
                    alert("🗑️ تم حذف السكريبت بنجاح!");
                });
            }
        }

        function switchTab(tab) {
            currentView = tab;
            document.getElementById('btn-all').className = tab === 'all' ? 'tab-btn active' : 'tab-btn';
            document.getElementById('btn-my').className = tab === 'my' ? 'tab-btn active' : 'tab-btn';
            renderScripts();
        }

        function listenToScripts() {
            db.ref('scripts').on('value', (snapshot) => {
                allScriptsData = snapshot.val() || {};
                renderScripts();
            });
        }

        function renderScripts() {
            let container = document.getElementById('scripts-container');
            container.innerHTML = '';
            
            let currentUser = localStorage.getItem('delta_active_user');
            let keys = Object.keys(allScriptsData);

            let filteredKeys = keys.filter(key => {
                let item = allScriptsData[key];
                if (currentView === 'my') {
                    return item.author === currentUser;
                }
                return true;
            });

            if (filteredKeys.length === 0) {
                container.innerHTML = `<p style="color: #777; margin-top: 20px;">${currentView === 'my' ? 'لم تقم بنشر أي سكريبتات للتحكم بها.' : 'لا توجد سكريبتات منشورة حالياً.'}</p>`;
                return;
            }

            filteredKeys.reverse().forEach((key) => {
                let item = allScriptsData[key];
                let isOwner = (item.author === currentUser);
                
                let scriptDiv = document.createElement('div');
                scriptDiv.className = 'glass-box script-card';
                scriptDiv.innerHTML = `
                    <div class="badge">🔥 Delta Verified</div>
                    <h3 style="margin: 5px 0 10px 0; color: #fff; font-size: 17px;">${escapeHtml(item.title)}</h3>
                    <p style="font-size: 11px; color: #888; margin-bottom: 10px;">الناشر: <b style="color: #00ffcc;">${escapeHtml(item.author)}</b> | التاريخ: ${item.time}</p>
                    <div class="code-box" id="scr_${key}">${escapeHtml(item.code)}</div>
                    <button class="btn-neon" onclick="copyScript('scr_${key}')" style="padding: 8px; font-size: 14px;">📋 نسخ كود التنفيذ (Execute)</button>
                    ${isOwner ? `<button class="btn-neon btn-danger" onclick="deleteScript('${key}')" style="padding: 6px; font-size: 12px; margin-top: 8px;">🗑️ حذف السكريبت</button>` : ''}
                `;
                container.appendChild(scriptDiv);
            });
        }

        function copyScript(id) {
            var text = document.getElementById(id).innerText;
            navigator.clipboard.writeText(text);
            alert("✅ تم نسخ السكريبت! افتح برنامج Delta Executor والعب فوراً.");
        }

        function escapeHtml(text) {
            return text.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;");
        }

        window.onload = function() {
            let activeUser = localStorage.getItem('delta_active_user');
            if (activeUser) {
                loginSuccess(activeUser);
            }
        }
    </script>

</body>
</html>
