<!DOCTYPE html>
<html dir="rtl" lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>شحن جواهر فري فاير وشدات ببجي موبايل</title>
    <style>
        /* تنسيق عام للصفحة */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: sans-serif;
            background-color: #263238;
            color: #ECEFF1;
            line-height: 1.6;
            padding: 0;
            margin: 0;
            direction: rtl;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }

        /* العنوان الرئيسي */
        header {
            text-align: center;
            margin-bottom: 30px;
        }

        header h1 {
            color: #80DEEA;
            font-size: 28px;
            padding: 10px 0;
        }

        /* تنسيق الأقسام */
        .section {
            margin-bottom: 25px;
            padding: 15px;
            border-radius: 8px;
            background-color: rgba(255, 255, 255, 0.05);
        }

        .section h2 {
            color: #90CAF9;
            font-size: 20px;
            margin-bottom: 15px;
        }

        /* إخفاء الأقسام */
        .hidden {
            display: none;
        }

        /* أزرار اختيار اللعبة */
        .game-selection-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 20px;
        }

        .game-btn {
            background-color: #26A69A;
            color: #ECEFF1;
            border: none;
            border-radius: 8px;
            padding: 15px 30px;
            cursor: pointer;
            font-size: 18px;
            flex: 1;
            text-align: center;
        }

        .game-btn:hover {
            background-color: #00796B;
        }

        .game-btn.selected {
            background-color: #00ACC1;
        }

        /* أزرار اختيار الباقة */
        .package-row {
            display: flex;
            justify-content: space-around;
            margin-bottom: 15px;
        }

        .package-btn {
            background-color: #26A69A;
            color: #ECEFF1;
            border: none;
            border-radius: 8px;
            padding: 12px;
            margin: 5px;
            cursor: pointer;
            font-size: 16px;
            text-align: center;
            flex: 1;
            max-width: 150px;
        }

        .package-btn:hover {
            background-color: #00796B;
        }

        .package-btn.selected {
            background-color: #00796B;
        }

        /* أزرار اختيار طريقة الدفع */
        .payment-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        .payment-btn {
            background-color: #78909C;
            color: #ECEFF1;
            border: none;
            border-radius: 8px;
            padding: 12px 25px;
            cursor: pointer;
            font-size: 16px;
            width: 40%;
        }

        .payment-btn:hover {
            background-color: #00796B;
        }

        .payment-btn.selected {
            background-color: #00ACC1;
        }

        /* معلومات الدفع */
        .highlight-text {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 10px;
            border-radius: 5px;
            margin-bottom: 15px;
            color: #FFF59D;
            font-size: 18px;
        }

        #payment-details {
            margin-bottom: 20px;
            line-height: 1.8;
        }

        /* قسم التحذير */
        .warning-title {
            color: #FF8A65 !important;
        }

        .warning-text {
            color: #FFCC80;
            margin-bottom: 20px;
            font-size: 15px;
            line-height: 1.8;
        }

        .warning-btn {
            background-color: #FFB74D;
            color: #263238;
            border: none;
            border-radius: 8px;
            padding: 12px 20px;
            cursor: pointer;
            font-size: 16px;
            display: block;
            margin: 0 auto;
        }

        .warning-btn:hover {
            background-color: #FFA726;
        }

        /* حقول الإدخال */
        .input-field {
            width: 100%;
            padding: 12px;
            margin-bottom: 15px;
            border: none;
            border-radius: 5px;
            background-color: #37474F;
            color: #ECEFF1;
            font-size: 16px;
        }

        .input-field::placeholder {
            color: rgba(236, 239, 241, 0.6);
        }

        /* أزرار الإجراءات */
        .action-btn {
            background-color: #00796B;
            color: #ECEFF1;
            border: none;
            border-radius: 8px;
            padding: 12px 25px;
            cursor: pointer;
            font-size: 16px;
            display: block;
            margin: 0 auto;
            width: 80%;
        }

        .action-btn:hover {
            background-color: #00695C;
        }

        /* قسم التأكيد */
        .confirm-title {
            color: #AED581 !important;
        }

        .confirm-message {
            text-align: center;
            margin-bottom: 20px;
            font-size: 16px;
        }

        .order-summary {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
            line-height: 1.8;
        }

        .share-instructions {
            margin: 20px 0;
            padding: 15px;
            background-color: rgba(255, 255, 255, 0.05);
            border-radius: 5px;
        }

        .share-instructions h3 {
            color: #90CAF9;
            font-size: 18px;
            margin-bottom: 10px;
        }

        /* تصميم متجاوب للشاشات الصغيرة */
        @media (max-width: 600px) {
            .game-btn {
                padding: 10px 20px;
                font-size: 16px;
            }
            .package-row {
                flex-direction: column;
                align-items: center;
            }
            
            .package-btn {
                width: 80%;
                max-width: none;
                margin-bottom: 10px;
            }
            
            .payment-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .payment-btn {
                width: 80%;
                margin-bottom: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>شحن الألعاب</h1>
        </header>

        <!-- قسم اختيار اللعبة -->
        <section id="game-selection" class="section">
            <h2>1. اختر اللعبة:</h2>
            <div class="game-selection-buttons">
                <button id="freefire-btn" class="game-btn">شحن جواهر فري فاير</button>
                <button id="pubg-btn" class="game-btn">شحن شدات ببجي موبايل</button>
            </div>
        </section>

        <!-- قسم شحن جواهر فري فاير -->
        <section id="freefire-sections" class="hidden">
            <section id="freefire-package-selection" class="section">
                <h2>2. اختر باقة الجواهر:</h2>
                <div class="package-row">
                    <button class="package-btn" data-game="freefire" data-name="100+10 جوهرة" data-price="2,950 ج.س">
                        100+10 جوهرة<br>2,950 ج.س
                    </button>
                    <button class="package-btn" data-game="freefire" data-name="210+21 جوهرة" data-price="5,750 ج.س">
                        210+21 جوهرة<br>5,750 ج.س
                    </button>
                    <button class="package-btn" data-game="freefire" data-name="530+53 جوهرة" data-price="14,150 ج.س">
                        530+53 جوهرة<br>14,150 ج.س
                    </button>
                </div>
                <div class="package-row">
                    <button class="package-btn" data-game="freefire" data-name="1080+180 جوهرة" data-price="28,150 ج.س">
                        1080+180 جوهرة<br>28,150 ج.س
                    </button>
                    <button class="package-btn" data-game="freefire" data-name="2200+220 جوهرة" data-price="56,200 ج.س">
                        2200+220 جوهرة<br>56,200 ج.س
                    </button>
                </div>
            </section>
        </section>

        <!-- قسم شحن شدات ببجي موبايل -->
        <section id="pubg-sections" class="hidden">
            <section id="pubg-package-selection" class="section">
                <h2>2. اختر باقة الشدات:</h2>
                <div class="package-row">
                    <button class="package-btn" data-game="pubg" data-name="60 شدة" data-price="3,000 ج.س">
                        60 شدة<br>3,000 ج.س
                    </button>
                    <button class="package-btn" data-game="pubg" data-name="300+25 شدة" data-price="14,400 ج.س">
                        300+25 شدة<br>14,400 ج.س
                    </button>
                    <button class="package-btn" data-game="pubg" data-name="600+60 شدة" data-price="28,650 ج.س">
                        600+60 شدة<br>28,650 ج.س
                    </button>
                </div>
                <div class="package-row">
                    <button class="package-btn" data-game="pubg" data-name="1500+300 شدة" data-price="71,500 ج.س">
                        1500+300 شدة<br>71,500 ج.س
                    </button>
                    <button class="package-btn" data-game="pubg" data-name="3000+850 شدة" data-price="142,900 ج.س">
                        3000+850 شدة<br>142,900 ج.س
                    </button>
                </div>
            </section>
        </section>

        <!-- قسم اختيار طريقة الدفع (مشترك بين اللعبتين) -->
        <section id="payment-method" class="section hidden">
            <h2>3. اختر طريقة الدفع:</h2>
            <div class="payment-buttons">
                <button id="bankak-btn" class="payment-btn" data-method="Bankak">بنكك</button>
                <button id="mykashy-btn" class="payment-btn" data-method="MyKashy">ماي كاشي</button>
            </div>
        </section>

        <!-- قسم معلومات الدفع (مشترك بين اللعبتين) -->
        <section id="payment-info" class="section hidden">
            <h2>4. معلومات الدفع:</h2>
            <div id="selected-package" class="highlight-text"></div>
            <div id="payment-details"></div>
            <button id="confirm-payment-btn" class="action-btn">لقد قمت بالدفع، متابعة</button>
        </section>

        <!-- قسم التحذير (مشترك بين اللعبتين) -->
        <section id="warning-section" class="section hidden">
            <h2 class="warning-title">5. تنبيه هام جداً: ⚠</h2>
            <p class="warning-text">
                أنت المسؤول الوحيد عن صحة معرف الحساب (ID) واسم الحساب اللذين تقوم بإدخالهما. 
                في حال إدخال معلومات خاطئة، لن نتمكن من استرجاع المبلغ أو إعادة عملية الشحن. 
                يرجى التأكد من البيانات بدقة قبل الإدخال.
            </p>
            <button id="accept-warning-btn" class="warning-btn">أوافق وأرغب في المتابعة لإدخال البيانات</button>
        </section>

        <!-- قسم إدخال بيانات الحساب (مشترك بين اللعبتين) -->
        <section id="account-input" class="section hidden">
            <h2 id="account-input-title">6. أدخل بيانات حسابك:</h2>
            <input type="number" id="player-id" placeholder="معرف الحساب (ID)" class="input-field">
            <input type="text" id="player-name" placeholder="اسم الحساب في اللعبة" class="input-field">
            <p style="font-size: 14px; color: #FFEB3B; margin-top: -10px; margin-bottom: 15px;">ملاحظة هامة: يرجى التأكد من صحة ID الحساب واسم الحساب في اللعبة لتجنب أي أخطاء في عملية الشحن.</p>
            <div id="full-name-input">
                <input type="text" id="full-name" placeholder="اسمك الرباعي (لمطابقة الدفع)" class="input-field">
                <p style="font-size: 14px; color: #BBDEFB; margin-top: -10px; margin-bottom: 15px;">يرجى إدخال اسمك الرباعي لضمان مطابقة الدفع وتجنب تشابه الأسماء.</p>
                <p style="font-size: 14px; color: #FFEB3B; margin-top: -10px; margin-bottom: 15px;">ملاحظة هامة: يجب أن يكون الاسم المدخل هو اسمك الحقيقي الرباعي. هذا ضروري لعملية الشحن ولن يتم استخدام معلوماتك إلا لهذا الغرض وبكل خصوصية.</p>
            </div>
            <button id="submit-order-btn" class="action-btn">إرسال الطلب الآن</button>
        </section>

        <!-- قسم تأكيد الطلب (مشترك بين اللعبتين) -->
        <section id="confirmation" class="section hidden">
            <h2 class="confirm-title">7. حالة الطلب:</h2>
            <div id="confirm-message" class="confirm-message">
                شكراً لك! لقد تم استلام طلبك بنجاح.
                سيتم شحن حسابك بعد التحقق من عملية الدفع.
                <br>
                <span style="color: #FFEB3B; font-weight: bold;">يرجى العلم أن الشحن سيصل في غضون ساعة إلى يوم كحد أقصى. نرجو منك التحلي بالصبر.</span>
                <br><br>
                <span style="color: #FFEB3B; font-weight: bold;">في حال عدم وصول الشحن بعد يوم، يرجى التواصل معنا عبر الواتساب على الرقم: <a href="https://wa.me/249912847087" target="_blank" style="color: #FFEB3B; text-decoration: underline;">0912847087</a> للمساعدة.</span>
            </div>
            <div id="order-summary" class="order-summary"></div>
            <div class="share-instructions">
                <h3>لإرسال تفاصيل الطلب:</h3>
                <p>
                    تم إرسال تفاصيل الطلب إلى نظامنا. 
                    يرجى أخذ لقطة شاشة لهذه الصفحة كمرجع.
                </p>
            </div>
            <button id="new-order-btn" class="action-btn">تقديم طلب جديد</button>
        </section>
    </div>

    <script>
        // المتغيرات العامة
        let selectedGame = "";
        let selectedPackageName = "";
        let selectedPackagePrice = "";
        let selectedPaymentMethod = "";
        let playerID = "";
        let playerName = "";
        let fullName = "";

        // أرقام الحسابات
        const bankakAccountNumber = "3312545";
        const myKashyAccountNumber = "400701521";

        // معلومات تليجرام (استبدلها بمعلوماتك)
        const TELEGRAM_BOT_TOKEN = "8099904195:AAEWJ6WwfZ4QExmehQCOLisWVBL95S0yfsk";
        const TELEGRAM_CHAT_ID = "7427451229";

        // عناصر DOM
        document.addEventListener("DOMContentLoaded", function() {
            // أزرار اختيار اللعبة
            const freefireBtn = document.getElementById("freefire-btn");
            const pubgBtn = document.getElementById("pubg-btn");
            freefireBtn.addEventListener("click", function() { selectGame("freefire", this); });
            pubgBtn.addEventListener("click", function() { selectGame("pubg", this); });

            // أزرار اختيار الباقة (فري فاير)
            const freefirePackageButtons = document.querySelectorAll("#freefire-sections .package-btn");
            freefirePackageButtons.forEach(button => {
                button.addEventListener("click", onPackageSelected);
            });

            // أزرار اختيار الباقة (ببجي موبايل)
            const pubgPackageButtons = document.querySelectorAll("#pubg-sections .package-btn");
            pubgPackageButtons.forEach(button => {
                button.addEventListener("click", onPackageSelected);
            });

            // أزرار اختيار طريقة الدفع
            const bankakButton = document.getElementById("bankak-btn");
            const myKashyButton = document.getElementById("mykashy-btn");
            bankakButton.addEventListener("click", function() {
                selectPaymentMethod("Bankak", this);
            });
            myKashyButton.addEventListener("click", function() {
                selectPaymentMethod("MyKashy", this);
            });

            // زر تأكيد الدفع
            const confirmPaymentButton = document.getElementById("confirm-payment-btn");
            confirmPaymentButton.addEventListener("click", function() {
                // إخفاء قسم معلومات الدفع وإظهار قسم التحذير
                document.getElementById("payment-info").classList.add("hidden");
                document.getElementById("warning-section").classList.remove("hidden");
                document.getElementById("warning-section").scrollIntoView({ behavior: "smooth" });
            });

            // زر قبول التحذير
            const acceptWarningButton = document.getElementById("accept-warning-btn");
            acceptWarningButton.addEventListener("click", function() {
                // إخفاء قسم التحذير وإظهار قسم إدخال البيانات
                document.getElementById("warning-section").classList.add("hidden");
                document.getElementById("account-input").classList.remove("hidden");
                document.getElementById("account-input").scrollIntoView({ behavior: "smooth" });
            });

            // زر إرسال الطلب
            const submitOrderButton = document.getElementById("submit-order-btn");
            submitOrderButton.addEventListener("click", submitOrder);

            // زر طلب جديد
            const newOrderButton = document.getElementById("new-order-btn");
            newOrderButton.addEventListener("click", resetForm);

            // إخفاء حقل الاسم الرباعي افتراضياً
            document.getElementById("full-name-input").classList.add("hidden");
        });

        // وظيفة اختيار اللعبة
        function selectGame(game, button) {
            selectedGame = game;

            // إزالة التحديد من جميع أزرار اللعبة
            document.querySelectorAll(".game-btn").forEach(btn => {
                btn.classList.remove("selected");
            });
            // إضافة التحديد للزر المختار
            button.classList.add("selected");

            // إخفاء جميع أقسام اللعبتين
            document.getElementById("freefire-sections").classList.add("hidden");
            document.getElementById("pubg-sections").classList.add("hidden");
            document.getElementById("payment-method").classList.add("hidden");
            document.getElementById("payment-info").classList.add("hidden");
            document.getElementById("warning-section").classList.add("hidden");
            document.getElementById("account-input").classList.add("hidden");
            document.getElementById("confirmation").classList.add("hidden");

            // إظهار القسم الخاص باللعبة المختارة
            if (selectedGame === "freefire") {
                document.getElementById("freefire-sections").classList.remove("hidden");
                document.getElementById("freefire-package-selection").scrollIntoView({ behavior: "smooth" });
            } else if (selectedGame === "pubg") {
                document.getElementById("pubg-sections").classList.remove("hidden");
                document.getElementById("pubg-package-selection").scrollIntoView({ behavior: "smooth" });
            }

            // مسح التحديد من الباقات وطرق الدفع عند تغيير اللعبة
            document.querySelectorAll(".package-btn").forEach(btn => {
                btn.classList.remove("selected");
            });
            document.querySelectorAll(".payment-btn").forEach(btn => {
                btn.classList.remove("selected");
            });

            // إعادة تعيين المتغيرات المتعلقة بالباقة والدفع
            selectedPackageName = "";
            selectedPackagePrice = "";
            selectedPaymentMethod = "";
            playerID = "";
            playerName = "";
            fullName = "";

            // إخفاء حقل الاسم الرباعي
            document.getElementById("full-name-input").classList.add("hidden");
        }

        // وظيفة عند اختيار الباقة
        function onPackageSelected(event) {
            const button = event.currentTarget;
            selectedPackageName = button.dataset.name;
            selectedPackagePrice = button.dataset.price;

            // إزالة التحديد من جميع أزرار الباقة لنفس اللعبة
            document.querySelectorAll(`#${selectedGame}-sections .package-btn`).forEach(btn => {
                btn.classList.remove("selected");
            });
            // إضافة التحديد للزر المختار
            button.classList.add("selected");

            // إظهار قسم طريقة الدفع
            document.getElementById("payment-method").classList.remove("hidden");
            document.getElementById("payment-method").scrollIntoView({ behavior: "smooth" });

            // مسح التحديد من طرق الدفع عند تغيير الباقة
            document.querySelectorAll(".payment-btn").forEach(btn => {
                btn.classList.remove("selected");
            });
            selectedPaymentMethod = "";

            // إخفاء الأقسام التالية
            document.getElementById("payment-info").classList.add("hidden");
            document.getElementById("warning-section").classList.add("hidden");
            document.getElementById("account-input").classList.add("hidden");
            document.getElementById("confirmation").classList.add("hidden");

            // إخفاء حقل الاسم الرباعي
            document.getElementById("full-name-input").classList.add("hidden");
        }

        // وظيفة اختيار طريقة الدفع
        function selectPaymentMethod(method, button) {
            selectedPaymentMethod = method;

            // إزالة التحديد من جميع أزرار الدفع
            document.querySelectorAll(".payment-btn").forEach(btn => {
                btn.classList.remove("selected");
            });
            // إضافة التحديد للزر المختار
            button.classList.add("selected");

            // تحديث وعرض معلومات الدفع
            updatePaymentInfo();

            // إظهار قسم معلومات الدفع
            document.getElementById("payment-info").classList.remove("hidden");
            document.getElementById("payment-info").scrollIntoView({ behavior: "smooth" });

            // إخفاء الأقسام التالية
            document.getElementById("warning-section").classList.add("hidden");
            document.getElementById("account-input").classList.add("hidden");
            document.getElementById("confirmation").classList.add("hidden");

            // إخفاء حقل الاسم الرباعي
            document.getElementById("full-name-input").classList.add("hidden");
        }

        // وظيفة تحديث معلومات الدفع
        function updatePaymentInfo() {
            const selectedPackageDiv = document.getElementById("selected-package");
            const paymentDetailsDiv = document.getElementById("payment-details");

            selectedPackageDiv.innerHTML = `لقد اخترت: <span style="color: #AED581;">${selectedPackageName}</span> بسعر: <span style="color: #AED581;">${selectedPackagePrice}</span>`;

            let details = "";
            if (selectedPaymentMethod === "Bankak") {
                details = `
                    <p>يرجى تحويل المبلغ إلى حساب بنكك التالي:</p>
                    <p style="font-weight: bold;">رقم الحساب: ${bankakAccountNumber}</p>
                    <p>اسم المستفيد: [اسم المستفيد بنكك]</p>
                    <p style="color: #FFEB3B;">ملاحظة: بعد التحويل، اضغط على زر "لقد قمت بالدفع، متابعة" أدناه.</p>
                `;
                document.getElementById("full-name-input").classList.remove("hidden");
            } else if (selectedPaymentMethod === "MyKashy") {
                details = `
                    <p>يرجى تحويل المبلغ إلى حساب ماي كاشي التالي:</p>
                    <p style="font-weight: bold;">رقم الحساب: ${myKashyAccountNumber}</p>
                    <p>اسم المستفيد: [اسم المستفيد ماي كاشي]</p>
                    <p style="color: #FFEB3B;">ملاحظة: بعد التحويل، اضغط على زر "لقد قمت بالدفع، متابعة" أدناه.</p>
                `;
                document.getElementById("full-name-input").classList.remove("hidden");
            }
            paymentDetailsDiv.innerHTML = details;
        }

        // وظيفة إرسال الطلب
        async function submitOrder() {
            playerID = document.getElementById("player-id").value;
            playerName = document.getElementById("player-name").value;
            fullName = document.getElementById("full-name").value;

            if (!playerID || !playerName || !fullName) {
                alert("الرجاء ملء جميع الحقول المطلوبة (معرف الحساب، اسم الحساب، الاسم الرباعي).");
                return;
            }

            // إخفاء جميع الأقسام
            document.getElementById("game-selection").classList.add("hidden");
            document.getElementById("freefire-sections").classList.add("hidden");
            document.getElementById("pubg-sections").classList.add("hidden");
            document.getElementById("payment-method").classList.add("hidden");
            document.getElementById("payment-info").classList.add("hidden");
            document.getElementById("warning-section").classList.add("hidden");
            document.getElementById("account-input").classList.add("hidden");

            // إظهار قسم التأكيد فقط
            document.getElementById("confirmation").classList.remove("hidden");
            document.getElementById("confirmation").scrollIntoView({ behavior: "smooth" });

            // تحديث ملخص الطلب
            const orderSummaryDiv = document.getElementById("order-summary");
            orderSummaryDiv.innerHTML = `
                <p>ملخص الطلب:</p>
                <p>اللعبة: <span style="color: #AED581;">${selectedGame === "freefire" ? "فري فاير" : "ببجي موبايل"}</span></p>
                <p>الباقة: <span style="color: #AED581;">${selectedPackageName}</span></p>
                <p>السعر: <span style="color: #AED581;">${selectedPackagePrice}</span></p>
                <p>طريقة الدفع: <span style="color: #AED581;">${selectedPaymentMethod}</span></p>
                <p>معرف الحساب: <span style="color: #AED581;">${playerID}</span></p>
                <p>اسم الحساب: <span style="color: #AED581;">${playerName}</span></p>
                <p>الاسم الرباعي: <span style="color: #AED581;">${fullName}</span></p>
            `;

            // إرسال البيانات إلى تليجرام
            const message = `
                طلب شحن جديد:
                اللعبة: ${selectedGame === "freefire" ? "فري فاير" : "ببجي موبايل"}
                الباقة: ${selectedPackageName}
                السعر: ${selectedPackagePrice}
                طريقة الدفع: ${selectedPaymentMethod}
                معرف الحساب: ${playerID}
                اسم الحساب: ${playerName}
                الاسم الرباعي: ${fullName}
            `;

            try {
                const response = await fetch(`https://api.telegram.org/bot${TELEGRAM_BOT_TOKEN}/sendMessage`, {
                    method: "POST",
                    headers: {
                        "Content-Type": "application/json"
                    },
                    body: JSON.stringify({
                        chat_id: TELEGRAM_CHAT_ID,
                        text: message
                    })
                });
                const data = await response.json();
                if (data.ok) {
                    console.log("Message sent to Telegram successfully!");
                } else {
                    console.error("Failed to send message to Telegram:", data);
                }
            } catch (error) {
                console.error("Error sending message to Telegram:", error);
            }
        }

        // وظيفة إعادة تعيين النموذج
        function resetForm() {
            // إخفاء جميع الأقسام ما عدا اختيار اللعبة
            document.getElementById("freefire-sections").classList.add("hidden");
            document.getElementById("pubg-sections").classList.add("hidden");
            document.getElementById("payment-method").classList.add("hidden");
            document.getElementById("payment-info").classList.add("hidden");
            document.getElementById("warning-section").classList.add("hidden");
            document.getElementById("account-input").classList.add("hidden");
            document.getElementById("confirmation").classList.add("hidden");

            // إظهار قسم اختيار اللعبة فقط
            document.getElementById("game-selection").classList.remove("hidden");

            // إزالة التحديد من أزرار اللعبة والباقة وطرق الدفع
            document.querySelectorAll(".game-btn").forEach(btn => {
                btn.classList.remove("selected");
            });
            document.querySelectorAll(".package-btn").forEach(btn => {
                btn.classList.remove("selected");
            });
            document.querySelectorAll(".payment-btn").forEach(btn => {
                btn.classList.remove("selected");
            });

            // مسح حقول الإدخال
            document.getElementById("player-id").value = "";
            document.getElementById("player-name").value = "";
            document.getElementById("full-name").value = "";

            // إعادة تعيين المتغيرات
            selectedGame = "";
            selectedPackageName = "";
            selectedPackagePrice = "";
            selectedPaymentMethod = "";
            playerID = "";
            playerName = "";
            fullName = "";

            // إخفاء حقل الاسم الرباعي
            document.getElementById("full-name-input").classList.add("hidden");

            // التمرير إلى أعلى الصفحة
            document.getElementById("game-selection").scrollIntoView({ behavior: "smooth" });
        }
    </script>
</body>
</html>
