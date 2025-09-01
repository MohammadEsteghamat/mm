# README.md — معادلات ماکسول و خلاصه‌ی امواج الکترومغناطیسی

این فایل خلاصه‌ای سازمان‌یافته از معادلات ماکسول، روابط ساختاری، معادلات موج، شرایط مرزی، پلاریزاسیون، بازتاب/شکست، بردار پوینتینگ و مفاهیم مرتبط با امواج هدایت‌شده است. تمام فرمول‌ها و توضیحات به زبان فارسی قرار گرفته‌اند.

---

## فهرست مطالب

1. معادلات ماکسول

   * فرم‌های نقطه‌ای و انتگرالی (استاتیک و دینامیک)
2. معادله پیوستگی
3. قضیه‌های برداری پایه
4. روابط ساختاری (Constitutive Relations)
5. معادلات موج

   * فضای آزاد
   * محیط رسانا
6. نماد فازور (Phasor Notation) و معادله هلمهولتز
7. انتشار موج در محیط‌های مختلف

   * محیط بدون تلفات
   * محیط رسانا (ثوابت انتشار، عمق نفوذ)
8. شرایط مرزی
9. پلاریزاسیون
10. بازتاب و شکست
11. بردار پوینتینگ و قضیه پوینتینگ
12. امواج هدایت‌شده (موجبرها و مودها)
13. مراجع / نکات پایانی

---

# 1. معادلات ماکسول

معادلات ماکسول اساس نظریهٔ میدان‌ها و امواج الکترومغناطیسی هستند. این معادلات به دو شکل نقطه‌ای (local / differential) و انتگرالی بیان می‌شوند.

## 1.1 معادلات ماکسول — میدان‌های استاتیک (فرم نقطه‌ای)

* $\nabla \times \vec{E} = 0$
* $\nabla \times \vec{H} = \vec{J}$  (قانون آمپر)
* $\nabla \cdot \vec{D} = \rho$  (قانون گاوس)
* $\nabla \cdot \vec{B} = 0$  (عدم وجود تک‌قطبی مغناطیسی)

## 1.2 معادلات ماکسول — میدان‌های استاتیک (فرم انتگرالی)

* $\displaystyle \oint_C \vec{E} \cdot d\vec{l} = 0$
* $\displaystyle \oint_C \vec{H} \cdot d\vec{l} = \iint_S \vec{J} \cdot d\vec{s}$
* $\displaystyle \oint_S \vec{D} \cdot d\vec{s} = \iiint_V \rho\, dV$
* $\displaystyle \oint_S \vec{B} \cdot d\vec{s} = 0$

## 1.3 معادلات ماکسول — میدان‌های دینامیک (فرم نقطه‌ای)

* $\nabla \times \vec{E} = - \dfrac{\partial \vec{B}}{\partial t}$  (قانون فاراده)
* $\nabla \times \vec{H} = \vec{J} + \dfrac{\partial \vec{D}}{\partial t}$  (قانون آمپر–ماکسول)
* $\nabla \cdot \vec{D} = \rho$
* $\nabla \cdot \vec{B} = 0$

## 1.4 معادلات ماکسول — میدان‌های دینامیک (فرم انتگرالی)

* $\displaystyle \oint_C \vec{E} \cdot d\vec{l} = - \iint_S \frac{\partial \vec{B}}{\partial t} \cdot d\vec{s}$
* $\displaystyle \oint_C \vec{H} \cdot d\vec{l} = \iint_S \left(\vec{J} + \frac{\partial \vec{D}}{\partial t}\right) \cdot d\vec{s}$
* $\displaystyle \oint_S \vec{D} \cdot d\vec{s} = \iiint_V \rho\, dV$
* $\displaystyle \oint_S \vec{B} \cdot d\vec{s} = 0$

**توضیحات نمادها:**

* $\vec{E}$: میدان الکتریکی
* $\vec{H}$: میدان مغناطیسی
* $\vec{J}$: چگالی جریان
* $\vec{D}$: چگالی شار الکتریکی (Electric flux density)
* $\rho$: چگالی بار
* $\vec{B}$: چگالی شار مغناطیسی (Magnetic flux density)

---

# 2. معادله پیوستگی

معادله پیوستگی که بقاى بار را بیان می‌کند:

$$
\nabla \cdot \vec{J} = - \frac{\partial \rho}{\partial t}
$$

این معادله نشان می‌دهد که کاهش بار در یک حجم با جریان خروجی از آن حجم برابر است.

---

# 3. قضیه‌های مهم برداری

* **قضیه استوکس (Stokes' Theorem)**:

$$
\oint_C \vec{F} \cdot d\vec{l} = \iint_S (\nabla \times \vec{F}) \cdot d\vec{s}
$$

* **قضیه دیورژانس (Divergence Theorem / Gauss's Theorem)**:

$$
\oint_S \vec{F} \cdot d\vec{s} = \iiint_V (\nabla \cdot \vec{F})\, dV
$$

این قضایا زیرساخت ریاضی معادلات ماکسول (انتگرال ↔ دیفرانسیل) هستند.

---

# 4. روابط ساختاری (Constitutive Relations)

روابطی که میدان‌ها را به خواص ماده ربط می‌دهند:

* $\vec{D} = \epsilon \vec{E}$
* $\vec{B} = \mu \vec{H}$
* $\vec{J} = \sigma \vec{E}$

که در آن $\epsilon = \epsilon_r \epsilon_0$ و $\mu = \mu_r \mu_0$ و $\sigma$ رسانندگی است. برای فضای آزاد: $\epsilon_r=1$, $\mu_r=1$, $\sigma=0$.

---

# 5. معادلات موج

با ترکیب معادلات ماکسول در فضای آزاد (بدون بار و جریان) به معادله موج برای میدان‌ها می‌رسیم:

* $\nabla^2 \vec{E} - \mu_0 \epsilon_0 \dfrac{\partial^2 \vec{E}}{\partial t^2} = 0$
* $\nabla^2 \vec{H} - \mu_0 \epsilon_0 \dfrac{\partial^2 \vec{H}}{\partial t^2} = 0$

سرعت انتشار در فضای آزاد:

$$
c = \frac{1}{\sqrt{\mu_0 \epsilon_0}} \approx 3 \times 10^8\ \mathrm{m/s}
$$

## 5.1 موج تخت یکنواخت (Uniform Plane Wave)

در موج تخت یکنواخت که در جهت مثلاً $x$ منتشر می‌شود، $\vec{E}$ و $\vec{H}$ عمود بر جهت انتشار هستند (موجِ عرضی):

$$
\frac{E_y}{H_z} = \sqrt{\frac{\mu}{\epsilon}} = \eta, \quad \frac{E_z}{H_y} = -\sqrt{\frac{\mu}{\epsilon}} = -\eta
$$

امپدانس ذاتی محیط: $\eta = \sqrt{\dfrac{\mu}{\epsilon}}$. برای فضای آزاد $\eta_0 \approx 120\pi \approx 377\ \Omega$.

## 5.2 معادله موج در محیط رسانا

برای محیطی که $\sigma \ne 0$:

* $\nabla^2 \vec{E} - \mu \sigma \dfrac{\partial \vec{E}}{\partial t} - \mu \epsilon \dfrac{\partial^2 \vec{E}}{\partial t^2} = 0$
* $\nabla^2 \vec{H} - \mu \sigma \dfrac{\partial \vec{H}}{\partial t} - \mu \epsilon \dfrac{\partial^2 \vec{H}}{\partial t^2} = 0$

---

# 6. نماد فازور (Phasor Notation)

برای تحلیل سینوسی زمانی با فرکانس ثابت $\omega$، مشتق زمانی با $j\omega$ جایگزین می‌شود.

معادلات ماکسول در دامنهٔ فازور:

* $\nabla \times \vec{E} = -j\omega \vec{B}$
* $\nabla \times \vec{H} = \vec{J} + j\omega \vec{D}$
* $\nabla \cdot \vec{D} = \rho$
* $\nabla \cdot \vec{B} = 0$

معادله هلمهولتز (Helmholtz) در فرم فازور برای محیط رسانا:

* $\nabla^2 \vec{E} - \gamma^2 \vec{E} = 0$
* $\nabla^2 \vec{H} - \gamma^2 \vec{H} = 0$

ثابت انتشار $\gamma$ تعریف می‌شود به صورت:

$$
\gamma = \sqrt{j\omega \mu (\sigma + j\omega \epsilon)} = \alpha + j\beta
$$

که $\alpha$ ثابت تضعیف و $\beta$ ثابت فاز است.

---

# 7. انتشار موج در محیط‌های مختلف

## 7.1 محیط بدون تلفات (Lossless)

اگر $\sigma = 0$، آنگاه $\gamma = j\beta$ و $\alpha = 0$:

$$
\beta = \omega \sqrt{\mu \epsilon}
$$

سرعت فاز:

$$
v_p = \frac{\omega}{\beta} = \frac{1}{\sqrt{\mu \epsilon}}
$$

طول موج:

$$
\lambda = \frac{2\pi}{\beta} = \frac{v_p}{f}
$$

## 7.2 محیط رسانا (Conducting Medium)

در حالت کلی $\alpha$ و $\beta$ برابرند با:

$$
\alpha = \omega \sqrt{\frac{\mu \epsilon}{2} \left( \sqrt{1 + \left(\frac{\sigma}{\omega \epsilon}\right)^2} - 1 \right)}
$$

$$
\beta = \omega \sqrt{\frac{\mu \epsilon}{2} \left( \sqrt{1 + \left(\frac{\sigma}{\omega \epsilon}\right)^2} + 1 \right)}
$$

امپدانس ذاتی محیط رسانا:

$$
\eta = \sqrt{\frac{j\omega \mu}{\sigma + j\omega \epsilon}}
$$

عمق نفوذ (Skin depth) $\delta$ و تقریب برای هادی‌های خوب ($\sigma \gg \omega \epsilon$):

$$
\delta = \frac{1}{\alpha}, \quad \alpha \approx \beta \approx \sqrt{\frac{\omega \mu \sigma}{2}}, \quad \delta \approx \sqrt{\frac{2}{\omega \mu \sigma}}
$$

---

# 8. شرایط مرزی (Boundary Conditions)

شرایط مرزی مولفه‌های مماسی و عمودی میدان‌ها را در مرز بین دو محیط مشخص می‌کنند.

## 8.1 مولفه‌های مماسی

* میدان الکتریکی مماسی پیوسته است (در غیاب تغییرات سطحی):

$$
E_{t1} = E_{t2}
$$

* میدان مغناطیسی مماسی پیوسته است مگر وجود جریان سطحی $J_s$:

$$
\vec{n} \times (\vec{H}_2 - \vec{H}_1) = \vec{J}_s
$$

اگر $J_s = 0$، آنگاه $H_{t1} = H_{t2}$.

## 8.2 مولفه‌های عمودی

* مولفه عمودیِ $\vec{D}$ پیوسته است مگر وجود چگالی بار سطحی $\rho_s$:

$$
\vec{n} \cdot (\vec{D}_2 - \vec{D}_1) = \rho_s
$$

* مولفه عمودیِ $\vec{B}$ همیشه پیوسته است:

$$
\vec{n} \cdot (\vec{B}_2 - \vec{B}_1) = 0
$$

## 8.3 شرایط برای هادی ایده‌آل (Perfect Conductor)

* داخل هادی ایده‌آل: $\vec{E} = 0$.
* مولفه مماسی میدان الکتریکی در سطح برابر صفر است: $E_t = 0$.
* مولفه عمودی $\vec{D}$ در سطح برابر چگالی بار سطحی $\rho_s$ است.
* مولفه مماسی $\vec{H}$ روی سطح برابر چگالی جریان سطحی $J_s$ است.

---

# 9. پلاریزاسیون (Polarization)

پلاریزاسیون رفتار بردار میدان الکتریکی در یک نقطهٔ مشخص در زمان را توصیف می‌کند.

* **خطی (Linear)**: مولفه‌ها هم‌فازند؛ بردار $\vec{E}$ در یک راستای ثابت نوسان می‌کند.
* **دایروی (Circular)**: دو مولفه با دامنهٔ برابر و اختلاف فاز $\pm 90^\circ$؛ مسیر نوک بردار $\vec{E}$ دایره است (راست‌گرد یا چپ‌گرد).
* **بیضوی (Elliptical)**: عمومی‌ترین حالت؛ دو مولفه با اختلاف فاز و دامنهٔ متفاوت که نوک بردار $\vec{E}$ بیضی رسم می‌کند.

---

# 10. بازتاب و شکست امواج (Reflection & Refraction)

## 10.1 برخورد عمودی

* **به هادی ایده‌آل**: بازتاب کامل؛ انرژی منتقل نمی‌شود.

  * $E_r = -E_i$  (تغییر فاز $180^\circ$ برای میدان الکتریکی)
  * $H_r = H_i$   (میدان مغناطیسی بدون تغییر فاز بازتاب می‌یابد)

* **به دی‌الکتریک ایده‌آل**:

  * ضریب بازتاب برای میدان الکتریکی:

  $$
  \Gamma_E = \frac{E_r}{E_i} = \frac{\eta_2 - \eta_1}{\eta_2 + \eta_1}
  $$

  * ضریب انتقال برای میدان الکتریکی:

  $$
  \mathcal{T}_E = \frac{E_t}{E_i} = \frac{2\eta_2}{\eta_1 + \eta_2}
  $$

  * ضریب بازتاب برای میدان مغناطیسی:

  $$
  \Gamma_H = \frac{H_r}{H_i} = \frac{\eta_1 - \eta_2}{\eta_1 + \eta_2}
  $$

  * ضریب انتقال برای میدان مغناطیسی:

  $$
  \mathcal{T}_H = \frac{H_t}{H_i} = \frac{2\eta_1}{\eta_1 + \eta_2}
  $$

## 10.2 برخورد مایل — قانون اسنل و زاویه بروستر

* **قانون اسنل (Snell's Law)**:

$$
\frac{\sin \theta_1}{\sin \theta_2} = \frac{v_1}{v_2} = \sqrt{\frac{\mu_2 \epsilon_2}{\mu_1 \epsilon_1}}
$$

* **زاویه بروستر (Brewster Angle)** برای پلاریزاسیون موازی:

$$
\tan \theta_B = \sqrt{\frac{\epsilon_2}{\epsilon_1}}
$$

---

# 11. بردار پوینتینگ و شار توان (Poynting)

**قضیه پوینتینگ (قانون بقای انرژی)**:

$$
(\nabla \cdot (\vec{E} \times \vec{H})) + \vec{E} \cdot \vec{J} + \frac{\partial}{\partial t} \left( \frac{1}{2} \epsilon \vec{E}^2 + \frac{1}{2} \mu \vec{H}^2 \right) = 0
$$

**بردار پوینتینگ (لحظه‌ای):**

$$
\vec{P} = \vec{E} \times \vec{H} \quad (\mathrm{W/m^2})
$$

**توان متوسط در فازور:**

$$
\vec{P}_{avg} = \frac{1}{2} \mathrm{Re} \{ \vec{E} \times \vec{H}^* \}
$$

---

# 12. امواج هدایت‌شده (Guided Waves)

امواجی که در امتداد یا روی سطوح هادی/دی‌الکتریک هدایت می‌شوند، مانند موجبرها و خطوط انتقال.

## 12.1 موجبر صفحه‌ای موازی (Parallel-Plate Waveguide)

دو صفحهٔ هادی موازی با فاصلهٔ $a$؛ مودهای اصلی:

1. **TE (Transverse Electric)**: $E_z = 0$. معادلهٔ موج برای $E_y$:

$$
\frac{\partial^2 E_y}{\partial x^2} + h^2 E_y = 0
$$

که $h = \dfrac{m\pi}{a}$ و فرکانس قطع:

$$
f_c = \frac{m}{2a\sqrt{\mu \epsilon}}
$$

2. **TM (Transverse Magnetic)**: $H_z = 0$. فرکانس قطع مشابه TE با قیدهای اندیس متفاوت.

3. **TEM (Transverse Electromagnetic)**: $E_z = H_z = 0$. فرکانس قطع برای TEM برابر با صفر است (هر فرکانسی می‌تواند منتشر شود).

**مود غالب برای موجبر صفحه‌ای:** معمولاً $TE_{10}$ یا پایین‌ترین مقدار m که امکان‌پذیر است.

## 12.2 موجبر مستطیلی (Rectangular Waveguide)

ابعاد $a \times b$ (با $a$ بزرگتر):

* **ثابت انتشار:**

$$
\gamma = \sqrt{\left(\frac{m\pi}{a}\right)^2 + \left(\frac{n\pi}{b}\right)^2 - \omega^2 \mu \epsilon}
$$

* **فرکانس قطع:**

$$
f_c = \frac{1}{2\pi \sqrt{\mu \epsilon}} \sqrt{\left(\frac{m\pi}{a}\right)^2 + \left(\frac{n\pi}{b}\right)^2} = \frac{1}{2} \sqrt{\frac{1}{\mu \epsilon}} \sqrt{\left(\frac{m}{a}\right)^2 + \left(\frac{n}{b}\right)^2}
$$

* **سرعت فاز:**

$$
v_p = \frac{\omega}{\beta} = \frac{1}{\sqrt{\mu \epsilon} \sqrt{1 - (f_c/f)^2}}
$$

(توجه: $v_p > c$ در موجبرها اما سرعت گروه $v_g < c$ و انرژی با سرعت گروه منتقل می‌شود.)

* **سرعت گروه:**

$$
v_g = c \sqrt{1 - (f_c/f)^2}
$$

و رابطهٔ مهم:

$$
v_p v_g = c^2
$$

* **طول موج در موجبر (Guide wavelength):**

$$
\lambda_g = \frac{2\pi}{\beta} = \frac{\lambda}{\sqrt{1 - (f_c/f)^2}}
$$

* **مودهای TE و TM:**

  * در موجبر مستطیلی، مود غالب معمولاً $TE_{10}$ است.
  * مودهای $TM_{mn}$ برای وجود نیاز به $m\ne 0$ و $n\ne 0$ دارند.

## 12.3 ضریب تضعیف در موجبرها (Attenuation)

تضعیف ناشی از مقاومت سطحی دیواره‌ها و تلفات دی‌الکتریک است.

* **برای موج TEM:**

$$
\alpha = \frac{R_s}{a\eta}
$$

که $R_s = \sqrt{\dfrac{\omega \mu_m}{2 \sigma_m}}$ مقاومت سطحی هادی است.

* **برای مود TE:**

$$
\alpha = \frac{R_s}{a\eta_w \beta} \left( \left(\frac{m\pi}{a}\right)^2 \frac{1}{\omega^2 \mu \epsilon} + \omega^2 \mu \epsilon \right)
$$

* **برای مود TM:** تضعیف در \$\$f = \sqrt{3} f\_c\$ حداقل است و سپس با فرکانس افزایش می‌یابد.

---

# 13. مراجع و نکات پایانی

این فایل یک خلاصهٔ جمع‌بندی از مفاهیم کلیدیِ مدار، میدان و امواج الکترومغناطیسی است و برای مرور سریع یا شروع مطالعهٔ عمیق‌تر مناسب است. اگر نیاز دارید:

* این فایل را به انگلیسی ترجمه کنم.
* مثال‌ها و مسائل حل‌شده (با مراحل کامل) اضافه کنم.
* یک نسخهٔ خلاصهٔ یک‌صفحه‌ای یا نقشهٔ ذهنی بسازم.

می‌توانید درخواست بعدی خود را همین‌جا بفرستید.

---

*تهیه‌شده با کمک خلاصهٔ ارائه‌شده توسط کاربر.*
