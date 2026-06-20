# TITIPIN_Elektronika-Dakwah
<!-- TITIPIN - Checkout -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>TITIPIN | Payment Method</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<style>
        body {
            font-family: 'Inter', sans-serif;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
        }
        .payment-option-input:checked + .payment-option-card {
            border-color: #236869;
            background-color: #f0fdfa;
            box-shadow: 0 0 0 1px #236869;
        }
        .payment-option-input:checked + .payment-option-card .check-icon {
            display: block;
        }
    </style>
<script id="tailwind-config">
        tailwind.config = {
          darkMode: "class",
          theme: {
            extend: {
              "colors": {
                      "surface": "#f8f9fa",
                      "on-primary": "#ffffff",
                      "surface-container-highest": "#e1e3e4",
                      "primary-container": "#1a2b3c",
                      "inverse-surface": "#2e3132",
                      "secondary-container": "#aaebec",
                      "secondary": "#236869",
                      "inverse-on-surface": "#f0f1f2",
                      "on-secondary": "#ffffff",
                      "inverse-primary": "#b7c8de",
                      "error": "#ba1a1a",
                      "on-tertiary-fixed": "#1b1c1c",
                      "outline-variant": "#c4c6cd",
                      "surface-bright": "#f8f9fa",
                      "tertiary-fixed": "#e4e2e1",
                      "primary-fixed": "#d2e4fb",
                      "surface-container": "#edeeef",
                      "on-tertiary": "#ffffff",
                      "surface-container-high": "#e7e8e9",
                      "tertiary-container": "#2a2a2a",
                      "outline": "#74777d",
                      "surface-tint": "#4f6073",
                      "on-secondary-fixed-variant": "#004f50",
                      "on-surface": "#191c1d",
                      "on-error-container": "#93000a",
                      "on-secondary-container": "#286c6d",
                      "on-primary-fixed": "#0b1d2d",
                      "surface-dim": "#d9dadb",
                      "tertiary-fixed-dim": "#c8c6c6",
                      "primary": "#041627",
                      "on-error": "#ffffff",
                      "background": "#f8f9fa",
                      "on-tertiary-fixed-variant": "#474747",
                      "tertiary": "#151516",
                      "on-tertiary-container": "#929190",
                      "primary-fixed-dim": "#b7c8de",
                      "surface-variant": "#e1e3e4",
                      "on-surface-variant": "#44474c",
                      "on-secondary-fixed": "#002020",
                      "on-background": "#191c1d",
                      "on-primary-container": "#8192a7",
                      "surface-container-low": "#f3f4f5",
                      "error-container": "#ffdad6",
                      "secondary-fixed": "#adeeef",
                      "secondary-fixed-dim": "#91d2d2",
                      "surface-container-lowest": "#ffffff",
                      "on-primary-fixed-variant": "#38485a"
              },
              "borderRadius": {
                      "DEFAULT": "0.25rem",
                      "lg": "0.5rem",
                      "xl": "0.75rem",
                      "full": "9999px"
              },
              "spacing": {
                      "margin-desktop": "48px",
                      "space-lg": "24px",
                      "gutter": "24px",
                      "margin-mobile": "16px",
                      "space-xl": "48px",
                      "space-xxl": "80px",
                      "space-md": "16px",
                      "container-max": "1280px",
                      "space-sm": "8px",
                      "unit": "8px",
                      "space-xs": "4px"
              },
              "fontFamily": {
                      "headline-lg": ["Inter"],
                      "label-md": ["Inter"],
                      "label-sm": ["Inter"],
                      "body-md": ["Inter"],
                      "body-lg": ["Inter"],
                      "display-lg-mobile": ["Inter"],
                      "headline-md": ["Inter"],
                      "display-lg": ["Inter"]
              },
              "fontSize": {
                      "headline-lg": ["32px", {"lineHeight": "40px", "fontWeight": "600"}],
                      "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "500"}],
                      "label-sm": ["12px", {"lineHeight": "16px", "letterSpacing": "0.05em", "fontWeight": "600"}],
                      "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                      "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}],
                      "display-lg-mobile": ["32px", {"lineHeight": "40px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                      "headline-md": ["24px", {"lineHeight": "32px", "fontWeight": "600"}],
                      "display-lg": ["48px", {"lineHeight": "56px", "letterSpacing": "-0.02em", "fontWeight": "700"}]
              }
            },
          },
        }
    </script>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
  </head>
<body class="bg-surface text-on-surface min-h-screen flex flex-col">
<!-- TopAppBar -->
<header class="fixed top-0 left-0 w-full z-50 bg-surface">
<div class="flex justify-between items-center w-full px-margin-mobile md:px-margin-desktop py-space-md max-w-container-max mx-auto">
<div class="flex items-center gap-space-md">
<button class="flex items-center justify-center w-10 h-10 hover:opacity-80 transition-opacity active:scale-95 duration-100 text-primary">
<span class="material-symbols-outlined">arrow_back</span>
</button>
<h1 class="text-headline-md font-headline-md font-bold text-primary">TITIPIN</h1>
</div>
<div class="w-10 h-10 rounded-full overflow-hidden bg-surface-container-highest border border-outline-variant/30">
<img alt="User Profile" class="w-full h-full object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuCCyU6J6AQo3y1DnV5StpCgbRmbFO3NcXaLwFaLHyk2Nh5G_sjolq5ZC2XUlyEGxUI9nI9zGwkFUznbRiHp2wSnP5ZaKbCmNLDDY2dkxIaWfK6RCVvbMrZmbLWzGXV9H8fJKYs2INNS864rrG6FnT_YxqxA5UcZBua49efWwiqdmQhLSRw4UB5d6trEcE-EoBm0sqxQ33birWFLblEkH6mCtNZwILOoaIjB-zH1-Uel6g8QjSxBg3rsuDBxJTcoGc5scEKGO1KrEap_"/>
</div>
</div>
</header>
<main class="flex-grow pt-24 pb-40 px-margin-mobile md:px-margin-desktop max-w-4xl mx-auto w-full">
<!-- Progress Stepper (Mobile Friendly) -->
<div class="mb-space-xl">
<div class="flex items-center justify-between relative">
<div class="absolute top-1/2 left-0 w-full h-0.5 bg-outline-variant -z-10 -translate-y-1/2"></div>
<div class="flex flex-col items-center gap-2 bg-surface px-2">
<div class="w-8 h-8 rounded-full bg-secondary text-on-secondary flex items-center justify-center text-label-sm">1</div>
<span class="text-label-sm font-label-sm text-secondary">Items</span>
</div>
<div class="flex flex-col items-center gap-2 bg-surface px-2">
<div class="w-8 h-8 rounded-full bg-secondary text-on-secondary flex items-center justify-center text-label-sm">2</div>
<span class="text-label-sm font-label-sm text-secondary">Details</span>
</div>
<div class="flex flex-col items-center gap-2 bg-surface px-2">
<div class="w-8 h-8 rounded-full bg-primary text-on-primary flex items-center justify-center text-label-sm">3</div>
<span class="text-label-sm font-label-sm text-primary">Payment</span>
</div>
</div>
</div>
<section class="space-y-space-lg">
<div class="space-y-1">
<h2 class="text-headline-md font-headline-md text-primary">Select Payment Method</h2>
<p class="text-body-md text-on-surface-variant">Choose a secure payment provider for your storage plan.</p>
</div>
<!-- Payment Options Grid -->
<div class="space-y-space-lg">
<!-- Bank Transfer Group -->
<div class="space-y-space-md">
<h3 class="text-label-md font-label-md text-outline uppercase tracking-wider">Bank Transfer</h3>
<div class="grid grid-cols-1 md:grid-cols-3 gap-space-md">
<!-- BCA -->
<label class="cursor-pointer relative">
<input checked="" class="hidden payment-option-input" name="payment_method" type="radio" value="bca"/>
<div class="payment-option-card h-full p-space-md bg-surface-container-lowest border border-outline-variant rounded-xl transition-all duration-200 hover:shadow-md flex flex-col justify-between items-start gap-4">
<div class="flex justify-between items-center w-full">
<div class="w-12 h-6 bg-blue-100 rounded-md flex items-center justify-center">
<span class="text-[10px] font-bold text-blue-800">BCA</span>
</div>
<span class="check-icon hidden text-secondary material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">check_circle</span>
</div>
<div class="space-y-1">
<p class="font-label-md text-label-md text-primary">BCA Virtual Account</p>
<p class="text-[12px] text-on-surface-variant">Instant verification 24/7</p>
</div>
</div>
</label>
<!-- Mandiri -->
<label class="cursor-pointer relative">
<input class="hidden payment-option-input" name="payment_method" type="radio" value="mandiri"/>
<div class="payment-option-card h-full p-space-md bg-surface-container-lowest border border-outline-variant rounded-xl transition-all duration-200 hover:shadow-md flex flex-col justify-between items-start gap-4">
<div class="flex justify-between items-center w-full">
<div class="w-12 h-6 bg-yellow-100 rounded-md flex items-center justify-center">
<span class="text-[10px] font-bold text-yellow-800">MANDIRI</span>
</div>
<span class="check-icon hidden text-secondary material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">check_circle</span>
</div>
<div class="space-y-1">
<p class="font-label-md text-label-md text-primary">Mandiri Bill Payment</p>
<p class="text-[12px] text-on-surface-variant">Secure bank-grade transfer</p>
</div>
</div>
</label>
<!-- BNI -->
<label class="cursor-pointer relative">
<input class="hidden payment-option-input" name="payment_method" type="radio" value="bni"/>
<div class="payment-option-card h-full p-space-md bg-surface-container-lowest border border-outline-variant rounded-xl transition-all duration-200 hover:shadow-md flex flex-col justify-between items-start gap-4">
<div class="flex justify-between items-center w-full">
<div class="w-12 h-6 bg-orange-100 rounded-md flex items-center justify-center">
<span class="text-[10px] font-bold text-orange-800">BNI</span>
</div>
<span class="check-icon hidden text-secondary material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">check_circle</span>
</div>
<div class="space-y-1">
<p class="font-label-md text-label-md text-primary">BNI Virtual Account</p>
<p class="text-[12px] text-on-surface-variant">Available for all branches</p>
</div>
</div>
</label>
</div>
</div>
<!-- E-wallet Group -->
<div class="space-y-space-md">
<h3 class="text-label-md font-label-md text-outline uppercase tracking-wider">E-Wallets</h3>
<div class="grid grid-cols-1 md:grid-cols-3 gap-space-md">
<!-- GoPay -->
<label class="cursor-pointer relative">
<input class="hidden payment-option-input" name="payment_method" type="radio" value="gopay"/>
<div class="payment-option-card h-full p-space-md bg-surface-container-lowest border border-outline-variant rounded-xl transition-all duration-200 hover:shadow-md flex flex-col justify-between items-start gap-4">
<div class="flex justify-between items-center w-full">
<div class="w-12 h-6 bg-teal-100 rounded-md flex items-center justify-center">
<span class="text-[10px] font-bold text-teal-800 uppercase">GoPay</span>
</div>
<span class="check-icon hidden text-secondary material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">check_circle</span>
</div>
<div class="space-y-1">
<p class="font-label-md text-label-md text-primary">GoPay</p>
<p class="text-[12px] text-on-surface-variant">Direct app redirection</p>
</div>
</div>
</label>
<!-- OVO -->
<label class="cursor-pointer relative">
<input class="hidden payment-option-input" name="payment_method" type="radio" value="ovo"/>
<div class="payment-option-card h-full p-space-md bg-surface-container-lowest border border-outline-variant rounded-xl transition-all duration-200 hover:shadow-md flex flex-col justify-between items-start gap-4">
<div class="flex justify-between items-center w-full">
<div class="w-12 h-6 bg-purple-100 rounded-md flex items-center justify-center">
<span class="text-[10px] font-bold text-purple-800 uppercase">OVO</span>
</div>
<span class="check-icon hidden text-secondary material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">check_circle</span>
</div>
<div class="space-y-1">
<p class="font-label-md text-label-md text-primary">OVO</p>
<p class="text-[12px] text-on-surface-variant">Pay with OVO Points or Cash</p>
</div>
</div>
</label>
<!-- Dana -->
<label class="cursor-pointer relative">
<input class="hidden payment-option-input" name="payment_method" type="radio" value="dana"/>
<div class="payment-option-card h-full p-space-md bg-surface-container-lowest border border-outline-variant rounded-xl transition-all duration-200 hover:shadow-md flex flex-col justify-between items-start gap-4">
<div class="flex justify-between items-center w-full">
<div class="w-12 h-6 bg-blue-100 rounded-md flex items-center justify-center">
<span class="text-[10px] font-bold text-blue-600 uppercase">DANA</span>
</div>
<span class="check-icon hidden text-secondary material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">check_circle</span>
</div>
<div class="space-y-1">
<p class="font-label-md text-label-md text-primary">DANA</p>
<p class="text-[12px] text-on-surface-variant">Quick checkout with DANA</p>
</div>
</div>
</label>
</div>
</div>
</div>
<!-- Bento Info Panel -->
<div class="grid grid-cols-1 md:grid-cols-2 gap-space-lg mt-space-xl">
<div class="p-space-lg bg-surface-container rounded-xl border border-outline-variant/30 flex items-start gap-space-md">
<span class="material-symbols-outlined text-secondary text-3xl">verified_user</span>
<div>
<h4 class="font-label-md text-label-md text-primary">Secure Transaction</h4>
<p class="text-body-md text-on-surface-variant text-sm">Your payment information is encrypted and never stored on our servers.</p>
</div>
</div>
<div class="p-space-lg bg-surface-container rounded-xl border border-outline-variant/30 flex items-start gap-space-md">
<span class="material-symbols-outlined text-secondary text-3xl">local_shipping</span>
<div>
<h4 class="font-label-md text-label-md text-primary">Pickup Protection</h4>
<p class="text-body-md text-on-surface-variant text-sm">Insurance coverage up to Rp 5.000.000 included for every storage plan.</p>
</div>
</div>
</div>
</section>
</main>
<!-- Bottom Sticky Summary & Action -->
<div class="fixed bottom-0 left-0 w-full bg-surface-container-lowest shadow-[0_-4px_12px_rgba(4,22,39,0.1)] border-t border-outline-variant/20 z-50">
<div class="max-w-container-max mx-auto px-margin-mobile md:px-margin-desktop py-space-md flex flex-col md:flex-row md:items-center justify-between gap-space-md">
<!-- Payment Summary Details -->
<div class="flex flex-col gap-1">
<div class="flex items-center gap-space-sm text-on-surface-variant">
<span class="text-label-sm font-label-sm uppercase tracking-tighter">Total Amount</span>
<button class="text-secondary" onclick="document.getElementById('details-modal').classList.toggle('hidden')">
<span class="material-symbols-outlined text-sm">info</span>
</button>
</div>
<div class="flex items-baseline gap-2">
<span class="text-headline-md font-headline-md text-primary">Rp 450.000</span>
<span class="text-label-sm font-label-sm text-outline">/ month</span>
</div>
</div>
<!-- Main Action -->
<div class="flex items-center gap-space-md">
<div class="hidden md:block text-right">
<p class="text-label-sm font-label-sm text-outline">Plan: Medium Unit (1.5m³)</p>
<p class="text-label-sm font-label-sm text-secondary">Pickup Scheduled: Oct 12, 10:00 AM</p>
</div>
<button class="flex-grow md:flex-none px-space-xl py-4 bg-primary text-on-primary rounded-xl font-headline-md text-lg shadow-lg hover:opacity-90 transition-all active:scale-[0.98] flex items-center justify-center gap-2">
                    Confirm &amp; Schedule Pickup
                    <span class="material-symbols-outlined">arrow_forward</span>
</button>
</div>
</div>
</div>
<!-- Hidden Order Details Modal (Toggleable for UI richness) -->
<div class="hidden fixed inset-0 z-[60] flex items-end md:items-center justify-center bg-primary/40 backdrop-blur-sm p-margin-mobile" id="details-modal">
<div class="bg-surface-container-lowest w-full max-w-md rounded-t-3xl md:rounded-3xl p-space-lg shadow-xl space-y-space-lg animate-in fade-in slide-in-from-bottom duration-300">
<div class="flex justify-between items-center">
<h3 class="text-headline-md font-headline-md text-primary">Order Summary</h3>
<button class="w-10 h-10 rounded-full bg-surface-container flex items-center justify-center" onclick="document.getElementById('details-modal').classList.add('hidden')">
<span class="material-symbols-outlined">close</span>
</button>
</div>
<div class="space-y-space-md">
<div class="flex justify-between items-center py-2 border-b border-outline-variant/30">
<span class="text-on-surface-variant">Medium Storage Unit</span>
<span class="font-semibold">Rp 350.000</span>
</div>
<div class="flex justify-between items-center py-2 border-b border-outline-variant/30">
<span class="text-on-surface-variant">Priority Pickup</span>
<span class="font-semibold">Rp 75.000</span>
</div>
<div class="flex justify-between items-center py-2 border-b border-outline-variant/30">
<span class="text-on-surface-variant">Basic Insurance</span>
<span class="font-semibold">Rp 25.000</span>
</div>
<div class="flex justify-between items-center pt-4">
<span class="text-headline-md font-headline-md">Total</span>
<span class="text-headline-md font-headline-md text-secondary">Rp 450.000</span>
</div>
</div>
<div class="p-space-md bg-secondary-container/30 rounded-xl flex items-center gap-3">
<span class="material-symbols-outlined text-secondary">auto_awesome</span>
<p class="text-label-sm font-label-sm text-on-secondary-container">Applied promo: STUDENT_MOVING (-Rp 0)</p>
</div>
<button class="w-full py-3 bg-secondary text-on-secondary rounded-xl font-label-md" onclick="document.getElementById('details-modal').classList.add('hidden')">
                Close Summary
            </button>
</div>
</div>
<!-- Background Decorative Element -->
<div class="fixed top-0 right-0 -z-10 opacity-5 w-[600px] h-[600px] pointer-events-none">
<div class="w-full h-full bg-gradient-to-bl from-secondary to-primary rounded-full blur-[120px]"></div>
</div>
<script>
        // Simple micro-interaction for payment selection
        const radioButtons = document.querySelectorAll('input[name="payment_method"]');
        radioButtons.forEach(radio => {
            radio.addEventListener('change', (e) => {
                // Potential for adding subtle haptic or sound feedback here
                console.log(`Selected payment: ${e.target.value}`);
            });
        });
    </script>
</body></html>

<!-- TITIPIN - Pricing & Promo -->
<!DOCTYPE html>

<html lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>TITIPIN | Pricing Estimate</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "surface": "#f8f9fa",
                        "on-primary": "#ffffff",
                        "surface-container-highest": "#e1e3e4",
                        "primary-container": "#1a2b3c",
                        "inverse-surface": "#2e3132",
                        "secondary-container": "#aaebec",
                        "secondary": "#236869",
                        "inverse-on-surface": "#f0f1f2",
                        "on-secondary": "#ffffff",
                        "inverse-primary": "#b7c8de",
                        "error": "#ba1a1a",
                        "on-tertiary-fixed": "#1b1c1c",
                        "outline-variant": "#c4c6cd",
                        "surface-bright": "#f8f9fa",
                        "tertiary-fixed": "#e4e2e1",
                        "primary-fixed": "#d2e4fb",
                        "surface-container": "#edeeef",
                        "on-tertiary": "#ffffff",
                        "surface-container-high": "#e7e8e9",
                        "tertiary-container": "#2a2a2a",
                        "outline": "#74777d",
                        "surface-tint": "#4f6073",
                        "on-secondary-fixed-variant": "#004f50",
                        "on-surface": "#191c1d",
                        "on-error-container": "#93000a",
                        "on-secondary-container": "#286c6d",
                        "on-primary-fixed": "#0b1d2d",
                        "surface-dim": "#d9dadb",
                        "tertiary-fixed-dim": "#c8c6c6",
                        "primary": "#041627",
                        "on-error": "#ffffff",
                        "background": "#f8f9fa",
                        "on-tertiary-fixed-variant": "#474747",
                        "tertiary": "#151516",
                        "on-tertiary-container": "#929190",
                        "primary-fixed-dim": "#b7c8de",
                        "surface-variant": "#e1e3e4",
                        "on-surface-variant": "#44474c",
                        "on-secondary-fixed": "#002020",
                        "on-background": "#191c1d",
                        "on-primary-container": "#8192a7",
                        "surface-container-low": "#f3f4f5",
                        "error-container": "#ffdad6",
                        "secondary-fixed": "#adeeef",
                        "secondary-fixed-dim": "#91d2d2",
                        "surface-container-lowest": "#ffffff",
                        "on-primary-fixed-variant": "#38485a"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.25rem",
                        "lg": "0.5rem",
                        "xl": "0.75rem",
                        "full": "9999px"
                    },
                    "spacing": {
                        "margin-desktop": "48px",
                        "space-lg": "24px",
                        "gutter": "24px",
                        "margin-mobile": "16px",
                        "space-xl": "48px",
                        "space-xxl": "80px",
                        "space-md": "16px",
                        "container-max": "1280px",
                        "space-sm": "8px",
                        "unit": "8px",
                        "space-xs": "4px"
                    },
                    "fontFamily": {
                        "headline-lg": ["Inter"],
                        "label-md": ["Inter"],
                        "label-sm": ["Inter"],
                        "body-md": ["Inter"],
                        "body-lg": ["Inter"],
                        "display-lg-mobile": ["Inter"],
                        "headline-md": ["Inter"],
                        "display-lg": ["Inter"]
                    },
                    "fontSize": {
                        "headline-lg": ["32px", {"lineHeight": "40px", "fontWeight": "600"}],
                        "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "500"}],
                        "label-sm": ["12px", {"lineHeight": "16px", "letterSpacing": "0.05em", "fontWeight": "600"}],
                        "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                        "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}],
                        "display-lg-mobile": ["32px", {"lineHeight": "40px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                        "headline-md": ["24px", {"lineHeight": "32px", "fontWeight": "600"}],
                        "display-lg": ["48px", {"lineHeight": "56px", "letterSpacing": "-0.02em", "fontWeight": "700"}]
                    }
                },
            },
        }
    </script>
<style>
        body { font-family: 'Inter', sans-serif; background-color: #f8f9fa; }
        .material-symbols-outlined { font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24; }
        .custom-shadow { box-shadow: 0 4px 12px rgba(4, 22, 39, 0.08); }
        .glass-card { background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(10px); border: 1px solid rgba(229, 231, 235, 1); }
        .promo-shimmer {
            background: linear-gradient(90deg, #236869 0%, #3caea3 50%, #236869 100%);
            background-size: 200% auto;
            animation: shimmer 3s linear infinite;
        }
        @keyframes shimmer { to { background-position: 200% center; } }
    </style>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
  </head>
<body class="bg-background text-on-surface min-h-screen pb-24">
<!-- Top Navigation -->
<header class="fixed top-0 left-0 w-full z-50 bg-surface">
<div class="flex justify-between items-center w-full px-margin-mobile md:px-margin-desktop py-space-md max-w-container-max mx-auto">
<button class="hover:opacity-80 transition-opacity active:scale-95 duration-100 flex items-center justify-center">
<span class="material-symbols-outlined text-primary text-[28px]">arrow_back</span>
</button>
<h1 class="text-headline-md font-headline-md font-extrabold text-primary tracking-tight">TITIPIN</h1>
<div class="w-10 h-10 rounded-full overflow-hidden border-2 border-outline-variant/30">
<img alt="User Profile" class="w-full h-full object-cover" data-alt="A professional close-up studio portrait of a young adult with a friendly expression. The lighting is soft and high-key, emphasizing a clean and modern aesthetic. The background is a solid, neutral off-white that matches a minimalist design system. The overall mood is trustworthy and academic, fitting a premium student service brand." src="https://lh3.googleusercontent.com/aida-public/AB6AXuDxaV2fVqsY-gkXTmAafYCD3t2cetbVxs6LVz8jayP1LmHVvTzKCVYMqILbhv6QjaIzUh01XydMOhUi8MqTu0cINMcvpvUjcUQXVO75SAkSTK75lU5o4ZpK_DgUvvdsLNEdVJGHcTTFsCcOkRKoeIiGwqhxcvOsBsb_uh3l-yi43Az4W3vcsMeefH-NXFiBMLqCwqBbvJ4lvl6-y2v9cMO7-DKuMuW-A8ydLw_fmzDLom5WtG06FVTlwl8atv8tDH5PolOjxIZMhtoX"/>
</div>
</div>
</header>
<main class="pt-24 px-margin-mobile md:px-margin-desktop max-w-[800px] mx-auto">
<!-- Success Animation Placeholder / Scene -->
<div class="mb-space-lg flex justify-center">
<div class="relative w-full max-w-md aspect-video rounded-xl overflow-hidden custom-shadow bg-primary-container">
<div class="absolute inset-0 flex flex-col items-center justify-center text-on-primary">
<span class="material-symbols-outlined text-[64px] mb-2 animate-bounce" style="font-variation-settings: 'FILL' 1;">check_circle</span>
<p class="text-label-md font-label-md uppercase tracking-widest opacity-80">Scan Complete</p>
</div>
<!-- Shimmering overlay effect -->
<div class="absolute inset-0 bg-gradient-to-tr from-primary/20 to-transparent pointer-events-none"></div>
</div>
</div>
<!-- Detected Items Summary Card -->
<section class="mb-space-lg">
<div class="glass-card rounded-xl p-space-lg custom-shadow">
<div class="flex items-center justify-between mb-space-md">
<h2 class="text-headline-md font-headline-md text-primary">Storage Summary</h2>
<span class="text-label-sm font-label-sm text-secondary bg-secondary-container px-3 py-1 rounded-full uppercase">3 Items Detected</span>
</div>
<div class="space-y-space-md">
<!-- Item Row 1 -->
<div class="flex items-center gap-space-md p-space-sm rounded-lg hover:bg-surface transition-colors border border-transparent hover:border-outline-variant/20">
<div class="w-12 h-12 bg-surface-container flex items-center justify-center rounded-lg">
<span class="material-symbols-outlined text-primary">luggage</span>
</div>
<div class="flex-1">
<p class="text-body-md font-semibold text-primary">Large Luggage</p>
<p class="text-label-sm text-on-surface-variant">Qty: 2 units • 80 x 50 x 30 cm</p>
</div>
<p class="text-body-md font-bold text-primary">Rp 100k</p>
</div>
<!-- Item Row 2 -->
<div class="flex items-center gap-space-md p-space-sm rounded-lg hover:bg-surface transition-colors border border-transparent hover:border-outline-variant/20">
<div class="w-12 h-12 bg-surface-container flex items-center justify-center rounded-lg">
<span class="material-symbols-outlined text-primary">inventory_2</span>
</div>
<div class="flex-1">
<p class="text-body-md font-semibold text-primary">Medium Box</p>
<p class="text-label-sm text-on-surface-variant">Qty: 1 unit • 40 x 40 x 40 cm</p>
</div>
<p class="text-body-md font-bold text-primary">Rp 50k</p>
</div>
</div>
</div>
</section>
<!-- Pricing Logic Section -->
<section class="mb-space-lg text-center">
<div class="py-space-xl px-space-lg bg-surface-container-lowest rounded-2xl border-2 border-primary/5 custom-shadow relative overflow-hidden">
<!-- Decorative background elements -->
<div class="absolute -top-10 -right-10 w-40 h-40 bg-secondary/5 rounded-full blur-3xl"></div>
<div class="absolute -bottom-10 -left-10 w-40 h-40 bg-primary/5 rounded-full blur-3xl"></div>
<p class="text-label-md font-label-md text-on-surface-variant uppercase tracking-widest mb-2">Estimated Total</p>
<h3 class="text-display-lg-mobile md:text-display-lg font-display-lg text-primary mb-2">
                    Your Monthly Storage: <span class="text-secondary">Rp 150.000</span>
</h3>
<div class="inline-flex items-center gap-2 bg-secondary/10 text-secondary px-4 py-2 rounded-full mb-4">
<span class="material-symbols-outlined text-[18px]">savings</span>
<p class="text-body-md font-medium">Much cheaper than your monthly boarding room rent!</p>
</div>
</div>
</section>
<!-- Promo Banner -->
<section class="mb-space-xl">
<div class="promo-shimmer rounded-xl p-space-md md:p-space-lg flex items-center justify-between text-on-secondary shadow-lg transform hover:scale-[1.01] transition-transform">
<div class="flex items-center gap-space-md">
<div class="w-12 h-12 bg-white/20 backdrop-blur-md rounded-full flex items-center justify-center">
<span class="material-symbols-outlined text-[28px]" style="font-variation-settings: 'FILL' 1;">celebration</span>
</div>
<div>
<h4 class="text-body-lg font-bold">Limited Time Offer!</h4>
<p class="text-label-md opacity-90">FREE pickup service for the first 1,000 users!</p>
</div>
</div>
<div class="hidden md:block">
<span class="material-symbols-outlined text-[48px] opacity-30">local_shipping</span>
</div>
</div>
</section>
<!-- Action Button -->
<div class="space-y-space-md">
<button class="w-full py-space-md bg-primary text-on-primary rounded-xl font-headline-md text-headline-md shadow-lg hover:opacity-90 active:scale-[0.98] transition-all flex items-center justify-center gap-2">
<span>Generate Invoice</span>
<span class="material-symbols-outlined">receipt_long</span>
</button>
<button class="w-full py-space-md border border-outline text-primary rounded-xl font-label-md text-label-md hover:bg-surface transition-colors">
                Recalculate Items
            </button>
</div>
<div class="mt-space-xl p-space-lg bg-surface-variant/30 rounded-xl border border-dashed border-outline-variant">
<div class="flex gap-space-md">
<span class="material-symbols-outlined text-outline">info</span>
<p class="text-label-sm text-on-surface-variant leading-relaxed">
                    This is an automated estimate based on AI-visual scanning. Final pricing will be confirmed by our team upon physical verification during pickup. Terms and conditions apply.
                </p>
</div>
</div>
</main>
<!-- Bottom Navigation Shell -->
<nav class="fixed bottom-0 left-0 w-full z-50 flex justify-around items-center bg-surface-container-lowest py-space-sm border-t border-outline-variant/20 shadow-[0_-4px_12px_rgba(4,22,39,0.1)] rounded-t-xl">
<a class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary transition-opacity" href="#">
<span class="material-symbols-outlined">home</span>
<span class="text-label-sm font-label-sm">Home</span>
</a>
<a class="flex flex-col items-center justify-center bg-secondary-container text-on-secondary-container rounded-full px-4 py-1 scale-90 transition-transform" href="#">
<span class="material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">document_scanner</span>
<span class="text-label-sm font-label-sm">Scan</span>
</a>
<a class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary transition-opacity" href="#">
<span class="material-symbols-outlined">receipt_long</span>
<span class="text-label-sm font-label-sm">Orders</span>
</a>
<a class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary transition-opacity" href="#">
<span class="material-symbols-outlined">person</span>
<span class="text-label-sm font-label-sm">Profile</span>
</a>
</nav>
<script>
        // Micro-interaction for the summary items
        document.querySelectorAll('.space-y-space-md > div').forEach(item => {
            item.addEventListener('mouseenter', () => {
                item.classList.add('translate-x-1');
            });
            item.addEventListener('mouseleave', () => {
                item.classList.remove('translate-x-1');
            });
        });
    </script>
</body></html>

<!-- TITIPIN - AI Scanning -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>TITIPIN | AI Object Scanning</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
        tailwind.config = {
          darkMode: "class",
          theme: {
            extend: {
              "colors": {
                      "surface": "#f8f9fa",
                      "on-primary": "#ffffff",
                      "surface-container-highest": "#e1e3e4",
                      "primary-container": "#1a2b3c",
                      "inverse-surface": "#2e3132",
                      "secondary-container": "#aaebec",
                      "secondary": "#236869",
                      "inverse-on-surface": "#f0f1f2",
                      "on-secondary": "#ffffff",
                      "inverse-primary": "#b7c8de",
                      "error": "#ba1a1a",
                      "on-tertiary-fixed": "#1b1c1c",
                      "outline-variant": "#c4c6cd",
                      "surface-bright": "#f8f9fa",
                      "tertiary-fixed": "#e4e2e1",
                      "primary-fixed": "#d2e4fb",
                      "surface-container": "#edeeef",
                      "on-tertiary": "#ffffff",
                      "surface-container-high": "#e7e8e9",
                      "tertiary-container": "#2a2a2a",
                      "outline": "#74777d",
                      "surface-tint": "#4f6073",
                      "on-secondary-fixed-variant": "#004f50",
                      "on-surface": "#191c1d",
                      "on-error-container": "#93000a",
                      "on-secondary-container": "#286c6d",
                      "on-primary-fixed": "#0b1d2d",
                      "surface-dim": "#d9dadb",
                      "tertiary-fixed-dim": "#c8c6c6",
                      "primary": "#041627",
                      "on-error": "#ffffff",
                      "background": "#f8f9fa",
                      "on-tertiary-fixed-variant": "#474747",
                      "tertiary": "#151516",
                      "on-tertiary-container": "#929190",
                      "primary-fixed-dim": "#b7c8de",
                      "surface-variant": "#e1e3e4",
                      "on-surface-variant": "#44474c",
                      "on-secondary-fixed": "#002020",
                      "on-background": "#191c1d",
                      "on-primary-container": "#8192a7",
                      "surface-container-low": "#f3f4f5",
                      "error-container": "#ffdad6",
                      "secondary-fixed": "#adeeef",
                      "secondary-fixed-dim": "#91d2d2",
                      "surface-container-lowest": "#ffffff",
                      "on-primary-fixed-variant": "#38485a"
              },
              "borderRadius": {
                      "DEFAULT": "0.25rem",
                      "lg": "0.5rem",
                      "xl": "0.75rem",
                      "full": "9999px"
              },
              "spacing": {
                      "margin-desktop": "48px",
                      "space-lg": "24px",
                      "gutter": "24px",
                      "margin-mobile": "16px",
                      "space-xl": "48px",
                      "space-xxl": "80px",
                      "space-md": "16px",
                      "container-max": "1280px",
                      "space-sm": "8px",
                      "unit": "8px",
                      "space-xs": "4px"
              },
              "fontFamily": {
                      "headline-lg": ["Inter"],
                      "label-md": ["Inter"],
                      "label-sm": ["Inter"],
                      "body-md": ["Inter"],
                      "body-lg": ["Inter"],
                      "display-lg-mobile": ["Inter"],
                      "headline-md": ["Inter"],
                      "display-lg": ["Inter"]
              },
              "fontSize": {
                      "headline-lg": ["32px", {"lineHeight": "40px", "fontWeight": "600"}],
                      "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "500"}],
                      "label-sm": ["12px", {"lineHeight": "16px", "letterSpacing": "0.05em", "fontWeight": "600"}],
                      "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                      "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}],
                      "display-lg-mobile": ["32px", {"lineHeight": "40px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                      "headline-md": ["24px", {"lineHeight": "32px", "fontWeight": "600"}],
                      "display-lg": ["48px", {"lineHeight": "56px", "letterSpacing": "-0.02em", "fontWeight": "700"}]
              }
            },
          },
        }
    </script>
<style>
        @keyframes scan-line {
            0% { transform: translateY(0); opacity: 0; }
            50% { opacity: 1; }
            100% { transform: translateY(320px); opacity: 0; }
        }
        .scan-anim {
            animation: scan-line 2.5s cubic-bezier(0.4, 0, 0.2, 1) infinite;
        }
        .mesh-bg {
            background-image: radial-gradient(circle, rgba(35, 104, 105, 0.1) 1px, transparent 1px);
            background-size: 24px 24px;
        }
        .glass-overlay {
            background: rgba(4, 22, 39, 0.7);
            backdrop-filter: blur(8px);
        }
        .detection-box {
            border: 2px solid #aaebec;
            box-shadow: 0 0 15px rgba(170, 235, 236, 0.4);
        }
    </style>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
  </head>
<body class="bg-surface font-body-md text-on-surface overflow-hidden">
<!-- Top Navigation (Shell Implementation) -->
<header class="fixed top-0 left-0 w-full z-50 bg-transparent flex justify-between items-center px-margin-mobile md:px-margin-desktop py-space-md max-w-container-max mx-auto">
<div class="flex items-center gap-space-sm">
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-white/20 backdrop-blur-md text-white hover:opacity-80 active:scale-95 transition-all">
<span class="material-symbols-outlined">arrow_back</span>
</button>
<h1 class="text-white font-bold font-headline-md text-headline-md tracking-tight">TITIPIN</h1>
</div>
<div class="flex items-center gap-space-md">
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-white/20 backdrop-blur-md text-white">
<span class="material-symbols-outlined">flash_on</span>
</button>
<button class="w-10 h-10 flex items-center justify-center rounded-full bg-white/20 backdrop-blur-md text-white">
<span class="material-symbols-outlined">flip_camera_ios</span>
</button>
</div>
</header>
<!-- Main Viewfinder Canvas -->
<main class="relative h-screen w-full bg-primary flex items-center justify-center overflow-hidden">
<!-- Viewfinder Image Placeholder -->
<div class="absolute inset-0 w-full h-full overflow-hidden">
<img class="w-full h-full object-cover opacity-80" data-alt="A clean minimalist room interior featuring organized storage boxes and stacked luggage in a corner. The lighting is soft and natural, emphasizing a professional and calm atmosphere. The shot is framed from a first-person perspective as if through a high-end smartphone camera lens, with a slight cinematic depth of field. The color palette is composed of cool blues, crisp whites, and deep navy accents, maintaining a premium tech-focused aesthetic." src="https://lh3.googleusercontent.com/aida-public/AB6AXuASIS_WFAuEfpBDUbueOXjY0FlEaFvPUQwehlA9HZUI4wIXQFff0PeCCwQLkVVJZhWMjH3R2P_jliJ5rfIBsqgd9SLxeQ5t8A9o2kUhOQk96zSF0dGG6J1Q7fab6wzehJcywNYkwyPSS-7PdX2QnzIKNEhto9eWOax0VFpOOPsSsRbal7aUI8DC7FWuuATEpp71TTMp0W44xzJ7AicpJh5T-tfU9A5UKMSBfc66Yp08vjibgNK7ftAX1jXW8PlCksPjLBpapBpQvV4U"/>
<!-- Scanning Mesh Overlay -->
<div class="absolute inset-0 mesh-bg opacity-30 pointer-events-none"></div>
</div>
<!-- Scanning Interface Elements -->
<div class="relative z-10 w-full max-w-md px-margin-mobile flex flex-col items-center">
<!-- AI Tracking Reticle -->
<div class="relative w-80 h-80 flex items-center justify-center">
<!-- Corner Brackets -->
<div class="absolute top-0 left-0 w-8 h-8 border-t-4 border-l-4 border-secondary rounded-tl-lg"></div>
<div class="absolute top-0 right-0 w-8 h-8 border-t-4 border-r-4 border-secondary rounded-tr-lg"></div>
<div class="absolute bottom-0 left-0 w-8 h-8 border-b-4 border-l-4 border-secondary rounded-bl-lg"></div>
<div class="absolute bottom-0 right-0 w-8 h-8 border-b-4 border-r-4 border-secondary rounded-br-lg"></div>
<!-- Animated Scan Line -->
<div class="absolute top-0 left-2 right-2 h-0.5 bg-secondary-container shadow-[0_0_10px_#aaebec] scan-anim"></div>
<!-- Floating Labels (Simulated Detection) -->
<div class="absolute -top-12 left-0 animate-bounce">
<div class="flex items-center gap-2 bg-secondary-container text-on-secondary-container px-3 py-1.5 rounded-full shadow-lg border border-secondary/20">
<span class="material-symbols-outlined text-[18px]">inventory_2</span>
<span class="font-label-md text-label-md">Large Suitcase detected</span>
</div>
</div>
<div class="absolute top-1/2 -right-16 transform -translate-y-1/2">
<div class="flex items-center gap-2 bg-white/90 backdrop-blur-md text-primary px-3 py-1.5 rounded-full shadow-lg border border-outline-variant/30">
<span class="material-symbols-outlined text-[18px]">straighten</span>
<span class="font-label-md text-label-md">75cm x 45cm</span>
</div>
</div>
<!-- Center Target -->
<div class="w-4 h-4 border-2 border-white rounded-full opacity-50"></div>
</div>
<!-- Guidance Text -->
<div class="mt-space-xl text-center">
<p class="text-white font-label-md text-label-md uppercase tracking-widest opacity-80 mb-2">Analyzing Volume</p>
<h2 class="text-white font-headline-md text-headline-md">Hold steady for estimate</h2>
</div>
</div>
<!-- Lower Interaction Panel -->
<div class="fixed bottom-0 left-0 w-full glass-overlay px-margin-mobile py-space-lg md:py-space-xl rounded-t-[2.5rem] flex flex-col items-center border-t border-white/10">
<div class="w-12 h-1.5 bg-white/20 rounded-full mb-space-lg"></div>
<div class="w-full max-w-container-max mx-auto flex flex-col gap-space-md">
<!-- Item Summary Strip -->
<div class="flex justify-between items-center bg-white/10 rounded-xl p-space-md">
<div class="flex items-center gap-space-md">
<div class="w-10 h-10 bg-secondary rounded-lg flex items-center justify-center text-white">
<span class="material-symbols-outlined">category</span>
</div>
<div>
<p class="text-white/60 text-label-sm font-label-sm uppercase">Item Class</p>
<p class="text-white font-body-md font-bold">Standard Storage Box</p>
</div>
</div>
<div class="text-right">
<p class="text-white/60 text-label-sm font-label-sm uppercase">Est. Cost</p>
<p class="text-secondary-fixed font-headline-md text-headline-md">Rp 15.000<span class="text-label-sm">/day</span></p>
</div>
</div>
<!-- Primary Action -->
<button class="w-full bg-secondary hover:bg-on-secondary-fixed-variant text-white py-4 rounded-xl flex items-center justify-center gap-3 active:scale-[0.98] transition-all group">
<span class="material-symbols-outlined group-hover:rotate-12 transition-transform">view_in_ar</span>
<span class="font-headline-md text-headline-md">Capture &amp; Estimate</span>
</button>
<p class="text-center text-white/40 text-label-sm font-label-sm px-10">
                    AI estimates are based on visible dimensions and may vary upon physical drop-off.
                </p>
</div>
<!-- Spacer for Bottom Nav Padding on Mobile -->
<div class="h-16 md:hidden"></div>
</div>
</main>
<!-- Bottom Navigation Shell (Consistent with JSON) -->
<nav class="fixed bottom-0 left-0 w-full z-50 flex justify-around items-center bg-surface-container-lowest dark:bg-inverse-surface py-space-sm border-t border-outline-variant/20 rounded-t-xl shadow-[0_-4px_12px_rgba(4,22,39,0.1)]">
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-outline-variant px-4 py-1 hover:text-secondary transition-opacity" href="#">
<span class="material-symbols-outlined">home</span>
<span class="text-label-sm font-label-sm">Home</span>
</a>
<a class="flex flex-col items-center justify-center bg-secondary-container dark:bg-on-secondary-fixed-variant text-on-secondary-container dark:text-secondary-fixed rounded-full px-4 py-1 scale-90 transition-transform" href="#">
<span class="material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">document_scanner</span>
<span class="text-label-sm font-label-sm">Scan</span>
</a>
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-outline-variant px-4 py-1 hover:text-secondary transition-opacity" href="#">
<span class="material-symbols-outlined">receipt_long</span>
<span class="text-label-sm font-label-sm">Orders</span>
</a>
<a class="flex flex-col items-center justify-center text-on-surface-variant dark:text-outline-variant px-4 py-1 hover:text-secondary transition-opacity" href="#">
<span class="material-symbols-outlined">person</span>
<span class="text-label-sm font-label-sm">Profile</span>
</a>
</nav>
<script>
        // Subtle micro-interaction: update label based on 'camera movement' simulation
        const detectionLabels = [
            "Large Suitcase detected",
            "Backpack detected",
            "Medium Storage Box",
            "Calculating dimensions...",
            "Checking storage availability"
        ];
        
        let labelIndex = 0;
        const mainLabel = document.querySelector('.animate-bounce .font-label-md');
        
        setInterval(() => {
            labelIndex = (labelIndex + 1) % detectionLabels.length;
            if(mainLabel) {
                mainLabel.style.opacity = '0';
                setTimeout(() => {
                    mainLabel.innerText = detectionLabels[labelIndex];
                    mainLabel.style.opacity = '1';
                }, 200);
            }
        }, 4000);

        // Flash interaction toggle simulation
        document.querySelectorAll('button').forEach(btn => {
            btn.addEventListener('mousedown', () => {
                btn.style.transform = 'scale(0.95)';
            });
            btn.addEventListener('mouseup', () => {
                btn.style.transform = 'scale(1)';
            });
        });
    </script>
</body></html>

<!-- TITIPIN - AI Invoice -->
<!DOCTYPE html>

<html lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8f9fa;
        }
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(8px);
            border: 1px solid rgba(229, 231, 235, 0.5);
        }
    </style>
<script id="tailwind-config">
        tailwind.config = {
          darkMode: "class",
          theme: {
            extend: {
              "colors": {
                      "surface": "#f8f9fa",
                      "on-primary": "#ffffff",
                      "surface-container-highest": "#e1e3e4",
                      "primary-container": "#1a2b3c",
                      "inverse-surface": "#2e3132",
                      "secondary-container": "#aaebec",
                      "secondary": "#236869",
                      "inverse-on-surface": "#f0f1f2",
                      "on-secondary": "#ffffff",
                      "inverse-primary": "#b7c8de",
                      "error": "#ba1a1a",
                      "on-tertiary-fixed": "#1b1c1c",
                      "outline-variant": "#c4c6cd",
                      "surface-bright": "#f8f9fa",
                      "tertiary-fixed": "#e4e2e1",
                      "primary-fixed": "#d2e4fb",
                      "surface-container": "#edeeef",
                      "on-tertiary": "#ffffff",
                      "surface-container-high": "#e7e8e9",
                      "tertiary-container": "#2a2a2a",
                      "outline": "#74777d",
                      "surface-tint": "#4f6073",
                      "on-secondary-fixed-variant": "#004f50",
                      "on-surface": "#191c1d",
                      "on-error-container": "#93000a",
                      "on-secondary-container": "#286c6d",
                      "on-primary-fixed": "#0b1d2d",
                      "surface-dim": "#d9dadb",
                      "tertiary-fixed-dim": "#c8c6c6",
                      "primary": "#041627",
                      "on-error": "#ffffff",
                      "background": "#f8f9fa",
                      "on-tertiary-fixed-variant": "#474747",
                      "tertiary": "#151516",
                      "on-tertiary-container": "#929190",
                      "primary-fixed-dim": "#b7c8de",
                      "surface-variant": "#e1e3e4",
                      "on-surface-variant": "#44474c",
                      "on-secondary-fixed": "#002020",
                      "on-background": "#191c1d",
                      "on-primary-container": "#8192a7",
                      "surface-container-low": "#f3f4f5",
                      "error-container": "#ffdad6",
                      "secondary-fixed": "#adeeef",
                      "secondary-fixed-dim": "#91d2d2",
                      "surface-container-lowest": "#ffffff",
                      "on-primary-fixed-variant": "#38485a"
              },
              "borderRadius": {
                      "DEFAULT": "0.25rem",
                      "lg": "0.5rem",
                      "xl": "0.75rem",
                      "full": "9999px"
              },
              "spacing": {
                      "margin-desktop": "48px",
                      "space-lg": "24px",
                      "gutter": "24px",
                      "margin-mobile": "16px",
                      "space-xl": "48px",
                      "space-xxl": "80px",
                      "space-md": "16px",
                      "container-max": "1280px",
                      "space-sm": "8px",
                      "unit": "8px",
                      "space-xs": "4px"
              },
              "fontFamily": {
                      "headline-lg": ["Inter"],
                      "label-md": ["Inter"],
                      "label-sm": ["Inter"],
                      "body-md": ["Inter"],
                      "body-lg": ["Inter"],
                      "display-lg-mobile": ["Inter"],
                      "headline-md": ["Inter"],
                      "display-lg": ["Inter"]
              },
              "fontSize": {
                      "headline-lg": ["32px", {"lineHeight": "40px", "fontWeight": "600"}],
                      "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "500"}],
                      "label-sm": ["12px", {"lineHeight": "16px", "letterSpacing": "0.05em", "fontWeight": "600"}],
                      "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                      "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}],
                      "display-lg-mobile": ["32px", {"lineHeight": "40px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                      "headline-md": ["24px", {"lineHeight": "32px", "fontWeight": "600"}],
                      "display-lg": ["48px", {"lineHeight": "56px", "letterSpacing": "-0.02em", "fontWeight": "700"}]
              }
            },
          },
        }
    </script>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
  </head>
<body class="bg-surface text-on-surface selection:bg-secondary-container">
<!-- Top AppBar (JSON Source of Truth) -->
<header class="fixed top-0 left-0 w-full z-50 bg-surface">
<div class="flex justify-between items-center w-full px-margin-mobile md:px-margin-desktop py-space-md max-w-container-max mx-auto">
<div class="flex items-center gap-space-md">
<button class="hover:opacity-80 transition-opacity active:scale-95 duration-100">
<span class="material-symbols-outlined text-primary">arrow_back</span>
</button>
<h1 class="text-headline-md font-headline-md font-bold text-primary">TITIPIN</h1>
</div>
<div class="flex items-center gap-space-md">
<div class="hidden md:flex gap-space-lg items-center px-space-lg">
<span class="text-on-surface-variant font-label-md text-label-md cursor-pointer hover:opacity-80">Home</span>
<span class="text-on-surface-variant font-label-md text-label-md cursor-pointer hover:opacity-80">Scan</span>
<span class="text-primary font-semibold font-label-md text-label-md cursor-pointer">Orders</span>
<span class="text-on-surface-variant font-label-md text-label-md cursor-pointer hover:opacity-80">Profile</span>
</div>
<div class="w-10 h-10 rounded-full bg-surface-container-highest overflow-hidden border border-outline-variant/30">
<img alt="User Profile" class="w-full h-full object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuCz2fvdCIkMFuP2zN3qL6O5hEBx1DNjn2Z6gFkMXRPjLSManykTWY4IlSYCG33cwNqHIjOovR8u0YrhwvRpYDZP_VcNOtT4h-FW13f_keLAM_1ddj7R_DjnHBzyry6oNESvF_Eh_pOgO4iqhAhEVz4cbyOmHW0WEMwrY8jRMsuO-vcsJjeM7nTtan8b2L1H2-p1qJc1WySkxWFGctCcz3Q0JsJxrG0H1hM4PqVKiODCv5eAHJyBCod13CZmxw9LZiCiQ_6yxr53CKEN"/>
</div>
</div>
</div>
</header>
<main class="pt-24 pb-32 px-margin-mobile md:px-margin-desktop max-w-[900px] mx-auto min-h-screen">
<!-- Header Section -->
<div class="mb-space-xl text-center md:text-left">
<span class="inline-block px-3 py-1 mb-space-sm rounded-full bg-secondary-container text-on-secondary-container font-label-sm text-label-sm">
                AI SCAN COMPLETE
            </span>
<h2 class="text-headline-lg font-headline-lg text-primary">AI Generated Invoice</h2>
<p class="text-on-surface-variant font-body-md text-body-md mt-space-xs">Review your storage breakdown and estimated logistics details.</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-12 gap-space-lg items-start">
<!-- Left Column: Order Details -->
<div class="md:col-span-7 space-y-space-lg">
<!-- Items Breakdown Card -->
<section class="bg-surface-container-lowest rounded-xl p-space-lg shadow-[0_4px_12px_rgba(4,22,39,0.05)] border border-outline-variant/20">
<div class="flex items-center gap-space-sm mb-space-md">
<span class="material-symbols-outlined text-secondary">inventory_2</span>
<h3 class="text-headline-md font-headline-md text-primary">Scanned Items</h3>
</div>
<div class="space-y-space-md">
<div class="flex justify-between items-center py-space-sm border-b border-outline-variant/10">
<div>
<p class="font-body-md text-body-md text-primary font-semibold">Large Storage Box</p>
<p class="text-label-sm font-label-sm text-on-surface-variant">Standard dimensions, heavy duty</p>
</div>
<span class="text-body-md font-body-md">x3</span>
</div>
<div class="flex justify-between items-center py-space-sm border-b border-outline-variant/10">
<div>
<p class="font-body-md text-body-md text-primary font-semibold">Medium Packing Crate</p>
<p class="text-label-sm font-label-sm text-on-surface-variant">Fragile handled items</p>
</div>
<span class="text-body-md font-body-md">x2</span>
</div>
<div class="flex justify-between items-center py-space-sm border-b border-outline-variant/10">
<div>
<p class="font-body-md text-body-md text-primary font-semibold">Furniture Piece</p>
<p class="text-label-sm font-label-sm text-on-surface-variant">Wrapped Study Desk (Small)</p>
</div>
<span class="text-body-md font-body-md">x1</span>
</div>
</div>
</section>
<!-- Duration & Logistics Card -->
<section class="bg-surface-container-lowest rounded-xl p-space-lg shadow-[0_4px_12px_rgba(4,22,39,0.05)] border border-outline-variant/20">
<div class="flex items-center gap-space-sm mb-space-md">
<span class="material-symbols-outlined text-secondary">schedule</span>
<h3 class="text-headline-md font-headline-md text-primary">Logistics Schedule</h3>
</div>
<div class="grid grid-cols-2 gap-space-md">
<div class="bg-surface-container-low p-space-md rounded-lg">
<p class="text-label-sm font-label-sm text-on-surface-variant uppercase tracking-wider mb-1">Duration</p>
<p class="font-headline-md text-headline-md text-primary">3 Months</p>
</div>
<div class="bg-surface-container-low p-space-md rounded-lg">
<p class="text-label-sm font-label-sm text-on-surface-variant uppercase tracking-wider mb-1">Pickup Est.</p>
<p class="font-headline-md text-headline-md text-primary">Oct 24, 09:00</p>
</div>
</div>
<div class="mt-space-md flex items-start gap-space-sm text-on-surface-variant">
<span class="material-symbols-outlined text-body-md">info</span>
<p class="text-label-md font-label-md">Our AI analyzed your items to optimize storage space and transport route efficiency.</p>
</div>
</section>
</div>
<!-- Right Column: Final Invoice (Receipt Aesthetic) -->
<div class="md:col-span-5">
<div class="bg-surface-container-lowest rounded-xl shadow-[0_12px_24px_rgba(4,22,39,0.08)] border border-outline-variant/30 overflow-hidden">
<!-- Receipt Header -->
<div class="bg-primary p-space-lg text-on-primary">
<p class="text-label-sm font-label-sm opacity-70 mb-1">INVOICE SUMMARY</p>
<div class="flex justify-between items-end">
<h4 class="text-headline-md font-headline-md">Order #TIT-7742</h4>
<span class="material-symbols-outlined">receipt_long</span>
</div>
</div>
<!-- Receipt Body -->
<div class="p-space-lg space-y-space-md relative">
<!-- Decorative Punch Holes -->
<div class="absolute -left-2 top-0 bottom-0 flex flex-col justify-around py-4 opacity-10">
<div class="w-4 h-4 bg-surface rounded-full"></div>
<div class="w-4 h-4 bg-surface rounded-full"></div>
<div class="w-4 h-4 bg-surface rounded-full"></div>
</div>
<div class="space-y-space-sm">
<div class="flex justify-between text-body-md font-body-md">
<span class="text-on-surface-variant">Items Total</span>
<span class="text-primary font-semibold">Rp 450.000</span>
</div>
<div class="flex justify-between text-body-md font-body-md">
<span class="text-on-surface-variant">Service Fee (AI Processing)</span>
<span class="text-primary font-semibold">Rp 10.000</span>
</div>
<div class="flex justify-between text-body-md font-body-md">
<span class="text-on-surface-variant">Pickup Logistics</span>
<span class="text-secondary font-bold">FREE</span>
</div>
</div>
<div class="border-t border-dashed border-outline-variant my-space-md"></div>
<div class="flex justify-between items-center py-space-sm">
<span class="text-headline-md font-headline-md text-primary">Total Amount</span>
<span class="text-headline-md font-headline-md text-primary">Rp 460.000</span>
</div>
<div class="pt-space-lg">
<button class="w-full bg-secondary hover:opacity-90 active:scale-95 transition-all text-on-secondary font-headline-md text-headline-md py-space-md rounded-xl flex items-center justify-center gap-space-sm">
                                Proceed to Payment
                                <span class="material-symbols-outlined">payments</span>
</button>
<p class="text-center text-label-sm font-label-sm text-on-surface-variant mt-space-md px-space-md">
                                Secure checkout via Bank Transfer or Digital Wallets.
                            </p>
</div>
</div>
<!-- Receipt Footer Pattern -->
<div class="h-4 w-full bg-[radial-gradient(circle_at_bottom,#f8f9fa_8px,transparent_8px)] bg-[length:16px_16px] bg-repeat-x"></div>
</div>
<!-- Visual Accent: Safe & Reliable -->
<div class="mt-space-lg flex items-center justify-center gap-space-sm text-on-surface-variant">
<span class="material-symbols-outlined text-secondary" style="font-variation-settings: 'FILL' 1;">verified_user</span>
<span class="text-label-md font-label-md">Insured &amp; Secure Storage Guaranteed</span>
</div>
</div>
</div>
</main>
<!-- Bottom Navigation Bar (Visible on Mobile Only) -->
<nav class="md:hidden fixed bottom-0 left-0 w-full z-50 flex justify-around items-center bg-surface-container-lowest py-space-sm border-t border-outline-variant/20 rounded-t-xl shadow-[0_-4px_12px_rgba(4,22,39,0.1)]">
<div class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary">
<span class="material-symbols-outlined">home</span>
<span class="text-label-sm font-label-sm">Home</span>
</div>
<div class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary">
<span class="material-symbols-outlined">document_scanner</span>
<span class="text-label-sm font-label-sm">Scan</span>
</div>
<!-- Active Tab: Orders -->
<div class="flex flex-col items-center justify-center bg-secondary-container text-on-secondary-container rounded-full px-4 py-1 active:scale-90 transition-transform">
<span class="material-symbols-outlined">receipt_long</span>
<span class="text-label-sm font-label-sm">Orders</span>
</div>
<div class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary">
<span class="material-symbols-outlined">person</span>
<span class="text-label-sm font-label-sm">Profile</span>
</div>
</nav>
<script>
        // Light Interaction logic
        document.querySelectorAll('button').forEach(button => {
            button.addEventListener('mousedown', () => {
                button.style.transform = 'scale(0.98)';
            });
            button.addEventListener('mouseup', () => {
                button.style.transform = 'scale(1)';
            });
        });

        // Subtle parallax or scroll effect could be added here
    </script>
</body></html>

<!-- TITIPIN - Home -->
<!DOCTYPE html><html class="light" lang="en" style=""><head>
<meta charset="utf-8">
<meta content="width=device-width, initial-scale=1.0" name="viewport">
<title>TITIPIN - Student Storage Simplified</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet">
<script id="tailwind-config">
        tailwind.config = {
          darkMode: "class",
          theme: {
            extend: {
              "colors": {
                      "surface": "#f8f9fa",
                      "on-primary": "#ffffff",
                      "surface-container-highest": "#e1e3e4",
                      "primary-container": "#1a2b3c",
                      "inverse-surface": "#2e3132",
                      "secondary-container": "#aaebec",
                      "secondary": "#236869",
                      "inverse-on-surface": "#f0f1f2",
                      "on-secondary": "#ffffff",
                      "inverse-primary": "#b7c8de",
                      "error": "#ba1a1a",
                      "on-tertiary-fixed": "#1b1c1c",
                      "outline-variant": "#c4c6cd",
                      "surface-bright": "#f8f9fa",
                      "tertiary-fixed": "#e4e2e1",
                      "primary-fixed": "#d2e4fb",
                      "surface-container": "#edeeef",
                      "on-tertiary": "#ffffff",
                      "surface-container-high": "#e7e8e9",
                      "tertiary-container": "#2a2a2a",
                      "outline": "#74777d",
                      "surface-tint": "#4f6073",
                      "on-secondary-fixed-variant": "#004f50",
                      "on-surface": "#191c1d",
                      "on-error-container": "#93000a",
                      "on-secondary-container": "#286c6d",
                      "on-primary-fixed": "#0b1d2d",
                      "surface-dim": "#d9dadb",
                      "tertiary-fixed-dim": "#c8c6c6",
                      "primary": "#041627",
                      "on-error": "#ffffff",
                      "background": "#f8f9fa",
                      "on-tertiary-fixed-variant": "#474747",
                      "tertiary": "#151516",
                      "on-tertiary-container": "#929190",
                      "primary-fixed-dim": "#b7c8de",
                      "surface-variant": "#e1e3e4",
                      "on-surface-variant": "#44474c",
                      "on-secondary-fixed": "#002020",
                      "on-background": "#191c1d",
                      "on-primary-container": "#8192a7",
                      "surface-container-low": "#f3f4f5",
                      "error-container": "#ffdad6",
                      "secondary-fixed": "#adeeef",
                      "secondary-fixed-dim": "#91d2d2",
                      "surface-container-lowest": "#ffffff",
                      "on-primary-fixed-variant": "#38485a"
              },
              "borderRadius": {
                      "DEFAULT": "0.25rem",
                      "lg": "0.5rem",
                      "xl": "0.75rem",
                      "full": "9999px"
              },
              "spacing": {
                      "margin-desktop": "48px",
                      "space-lg": "24px",
                      "gutter": "24px",
                      "margin-mobile": "16px",
                      "space-xl": "48px",
                      "space-xxl": "80px",
                      "space-md": "16px",
                      "container-max": "1280px",
                      "space-sm": "8px",
                      "unit": "8px",
                      "space-xs": "4px"
              },
              "fontFamily": {
                      "headline-lg": ["Inter"],
                      "label-md": ["Inter"],
                      "label-sm": ["Inter"],
                      "body-md": ["Inter"],
                      "body-lg": ["Inter"],
                      "display-lg-mobile": ["Inter"],
                      "headline-md": ["Inter"],
                      "display-lg": ["Inter"]
              },
              "fontSize": {
                      "headline-lg": ["32px", {"lineHeight": "40px", "fontWeight": "600"}],
                      "label-md": ["14px", {"lineHeight": "20px", "letterSpacing": "0.01em", "fontWeight": "500"}],
                      "label-sm": ["12px", {"lineHeight": "16px", "letterSpacing": "0.05em", "fontWeight": "600"}],
                      "body-md": ["16px", {"lineHeight": "24px", "fontWeight": "400"}],
                      "body-lg": ["18px", {"lineHeight": "28px", "fontWeight": "400"}],
                      "display-lg-mobile": ["32px", {"lineHeight": "40px", "letterSpacing": "-0.01em", "fontWeight": "700"}],
                      "headline-md": ["24px", {"lineHeight": "32px", "fontWeight": "600"}],
                      "display-lg": ["48px", {"lineHeight": "56px", "letterSpacing": "-0.02em", "fontWeight": "700"}]
              }
            },
          },
        }
    </script>
<style>
        body {
            background-color: #f8f9fa;
            color: #191c1d;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }
        .testimonial-scroll::-webkit-scrollbar {
            display: none;
        }
        .testimonial-scroll {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }
        .storage-card {
            transition: transform 0.2s cubic-bezier(0.4, 0, 0.2, 1), box-shadow 0.2s ease;
        }
        .storage-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 12px 24px rgba(4, 22, 39, 0.08);
            border-color: #236869;
        }
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
        }
    </style>
</head>
<body class="min-h-screen pb-32">
<!-- TopAppBar -->
<header class="fixed top-0 left-0 w-full z-50 bg-surface">
<div class="flex justify-between items-center w-full px-margin-mobile md:px-margin-desktop py-space-md max-w-container-max mx-auto">
<div class="flex items-center gap-space-sm">
<span class="material-symbols-outlined text-primary text-headline-md">arrow_back</span>
<h1 class="text-headline-md font-headline-md font-bold text-primary">TITIPIN</h1>
</div>
<div class="flex items-center gap-space-md">
<span class="text-label-md font-label-md text-on-surface-variant hidden md:block">Welcome, Alex</span>
<div class="w-10 h-10 rounded-full bg-surface-container-highest overflow-hidden border border-outline-variant">
<img alt="User Profile" class="w-full h-full object-cover" data-alt="A professional headshot of a friendly young adult male student with a modern haircut and stylish glasses. The photograph is shot in a bright, minimalist studio with a soft off-white background, matching a high-end corporate aesthetic. The lighting is soft and even, highlighting clear skin and a warm smile, conveying trust and reliability." src="https://lh3.googleusercontent.com/aida-public/AB6AXuB-d4sAkeRJwon_eOdiekkP4oUZDGosvs_019S8ej412klRExSd1qlXlP4Bcll07R1emM_xlroCir5ObtIJ0fRxM7WTPvDkgxaGbEeBhZ0aKChetoKGxkrktt73eutMWf2UxWbUzHhmp_eQvcVc-inC-kvQPO1ZmifMjzRVG4mIT5HPcUWrR2AEYnvhN6ZS3tIIkTblfxBdeDLqO8a58FuRFQWDKCkD-ifCZGf0AE6iIhnrf_F0mm5SDFPD2myyG0_5gAM7ecuopNda">
</div>
</div>
</div>
</header>
<main class="pt-24 max-w-container-max mx-auto px-margin-mobile md:px-margin-desktop">
<!-- Hero Greeting -->
<section class="mb-space-xl">
<h2 class="text-display-lg-mobile md:text-display-lg font-display-lg-mobile md:font-display-lg text-primary mb-space-xs">Hi, Alex!</h2>
<p class="text-body-lg text-on-surface-variant max-w-xl">Your transition just got easier. Select a storage option to secure your belongings.</p>
</section>
<!-- Bento Storage Grid -->
<section class="mb-space-xxl">
  <div class="bg-primary text-on-primary p-space-lg rounded-xl flex flex-col items-center text-center gap-space-md shadow-lg">
    <div class="w-16 h-16 bg-secondary-container rounded-full flex items-center justify-center mb-space-sm">
      <span class="material-symbols-outlined text-on-secondary-container text-[40px]" data-icon="document_scanner">document_scanner</span>
    </div>
    <h2 class="text-headline-lg font-headline-lg">Mulai Titip</h2>
    <p class="text-body-lg opacity-90 max-w-md">Gunakan AI kami untuk memindai barang-barang Anda dan dapatkan rekomendasi penyimpanan terbaik secara instan.</p>
    <button class="bg-secondary text-on-secondary px-space-xl py-space-md rounded-lg text-headline-md font-bold hover:opacity-90 transition-opacity mt-space-sm w-full md:w-auto">Mulai Titip Sekarang</button>
  </div>
</section>
<!-- Testimonial Section -->
<section class="mb-space-xl">
<div class="flex items-center justify-between mb-space-lg">
<h2 class="text-headline-lg font-headline-lg text-primary">Apa Kata Mahasiswa</h2>
<div class="flex gap-space-sm">
<button class="w-10 h-10 rounded-full border border-outline-variant flex items-center justify-center hover:bg-surface-container transition-colors" onclick="scrollTestimonials(-1)">
<span class="material-symbols-outlined" data-icon="chevron_left">chevron_left</span>
</button>
<button class="w-10 h-10 rounded-full border border-outline-variant flex items-center justify-center hover:bg-surface-container transition-colors" onclick="scrollTestimonials(1)">
<span class="material-symbols-outlined" data-icon="chevron_right">chevron_right</span>
</button>
</div>
</div>
<div class="testimonial-scroll flex overflow-x-auto gap-space-lg pb-space-md snap-x" id="testimonial-container">
<!-- Testimonial 1 -->
<div class="min-w-[300px] md:min-w-[400px] bg-surface-container-low p-space-lg rounded-xl snap-start">
<div class="flex items-center gap-space-md mb-space-md">
<img alt="Jordan" class="w-12 h-12 rounded-full border border-secondary" data-alt="Close up portrait of a college student with a joyful expression, wearing a casual denim jacket. The image is captured with shallow depth of field, blurring out a modern university campus background in daylight. The aesthetic is clean, academic, and highly professional, utilizing soft natural light and a navy and teal color scheme consistent with a premium educational brand." src="https://lh3.googleusercontent.com/aida-public/AB6AXuBBASl3qv5ZanqIM5_PAW2WrjGi5U2A-dauOLbldfOizG4nkFMOHT3ux0lVGwd4-ks5hxxCki5lVulNDSunhpL2077wHCv2AOk9sBJKaO48dJXRVmRPJaTkZQSkTqFQ5QsqNY0rGBAvOqezwDbb3oA_YrXjab9YhUBB0JACs1QH4YV7Yg_SqxTbI4wJqrCG1y6fCJvOS0IeHwq8IcgvHzcTnDgJ2-JwgLzM_Ec2aH_uGElDZP1qUan4OLeRW1gPUCqMPmtoMnmeVpC7">
<div>
<p class="text-label-md font-bold text-primary">Jordan Lee</p>
<p class="text-label-sm text-secondary">Stanford University</p>
</div>
</div>
<p class="text-body-md text-on-surface italic">"Sangat membantu untuk menghemat biaya sewa kos selama libur semester! Proses penjemputannya sangat lancar dan saya tidak perlu khawatir sama sekali."</p>
</div>
<!-- Testimonial 2 -->
<div class="min-w-[300px] md:min-w-[400px] bg-surface-container-low p-space-lg rounded-xl snap-start">
<div class="flex items-center gap-space-md mb-space-md">
<img alt="Sarah" class="w-12 h-12 rounded-full border border-secondary" data-alt="A portrait of a young female university student smiling warmly, set against a bright, airy library interior. The lighting is crisp and modern, emphasizing a minimalist and organized atmosphere. The composition uses high contrast and a clean color palette of off-white and deep navy, reflecting a trustworthy and efficient service provider for students." src="https://lh3.googleusercontent.com/aida-public/AB6AXuD2tH9GRIK3YxthrZyBYwC-FfuyrAcklB2TTZI5Pu6_WIXZRyN8aEdxsVWGasnS38RFgl9BOKtGyYo3mcbTEtdTA5NaacpkVLBaJGd17OeoccdHJd0nYBuwVnftKT071PBhXywnhRYJmJj4EMpG75y-qNEM6K4G_4b_8QFNpIUg8DmdVS67hMr585sYSugsT9Dvg7tMcytIvhnSfDuDEXyNfaZTPIQD3WXuVAzdvSe00m50dMT60zPjdbdr4MvP6nPTfGMvhyLVhVyY">
<div>
<p class="text-label-md font-bold text-primary">Sarah Chen</p>
<p class="text-label-sm text-secondary">MIT</p>
</div>
</div>
<p class="text-body-md text-on-surface italic">"Satu-satunya layanan penyimpanan yang saya percayai. Kotak TITIPIN sangat berkualitas dan sistem pelacakannya transparan. Sangat direkomendasikan untuk setiap mahasiswa."</p>
</div>
<!-- Testimonial 3 -->
<div class="min-w-[300px] md:min-w-[400px] bg-surface-container-low p-space-lg rounded-xl snap-start">
<div class="flex items-center gap-space-md mb-space-md">
<img alt="Marcus" class="w-12 h-12 rounded-full border border-secondary" data-alt="A smiling young male student with an approachable and reliable look, posed in front of a sleek, contemporary student housing building. The style is modern minimalism, with sharp focus and bright high-key lighting. The color palette emphasizes teal and navy accents, creating a sense of calm and institutional efficiency appropriate for a high-end moving service." src="https://lh3.googleusercontent.com/aida-public/AB6AXuCJnaFBseJyIXXLHE9WCu7tBCudbaWbb2_HhIOXFjxkHGSsxNpGeZbUFZhPErZKk59nRYyCL2zBUSbHwCVPlnLTEm3EOPX6KF8JM-YVHiExxbuNy5IGUob30E_pPYXFV4Dc0F99-NDGO-Da3an4QffVN_Ix2pQteYllfDDsiAbsQHPPLvMEAoV-sHduQegfFxz4ysqLWokijDKjkPY44xYNeRxYmaZ4DsJS6oPuA4hi6jXfXccSD7sczsWhHDoSoF8emRSUZtrXDMkf">
<div>
<p class="text-label-md font-bold text-primary">Marcus Wright</p>
<p class="text-label-sm text-secondary">UC Berkeley</p>
</div>
</div>
<p class="text-body-md text-on-surface italic">"Pindahan dulu selalu jadi mimpi buruk sampai saya menemukan TITIPIN. Profesional, efisien, dan sangat terjangkau untuk tingkat layanan yang diberikan."</p>
</div>
</div>
</section>
</main>
<!-- BottomNavBar -->
<nav class="fixed bottom-0 left-0 w-full z-50 flex justify-around items-center bg-surface-container-lowest py-space-sm border-t border-outline-variant/20 shadow-lg rounded-t-xl">
<!-- Home (Active) -->
<a class="flex flex-col items-center justify-center bg-secondary-container text-on-secondary-container rounded-full px-4 py-1 scale-90 transition-transform" href="#">
<span class="material-symbols-outlined" data-icon="home" style="font-variation-settings: 'FILL' 1;">home</span>
<span class="text-label-sm font-label-sm">Home</span>
</a>
<!-- Scan -->
<a class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="document_scanner">document_scanner</span>
<span class="text-label-sm font-label-sm">Scan</span>
</a>
<!-- Orders -->
<a class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="receipt_long">receipt_long</span>
<span class="text-label-sm font-label-sm">Orders</span>
</a>
<!-- Profile -->
<a class="flex flex-col items-center justify-center text-on-surface-variant px-4 py-1 hover:text-secondary transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="person">person</span>
<span class="text-label-sm font-label-sm">Profile</span>
</a>
</nav>
<script>
        function scrollTestimonials(direction) {
            const container = document.getElementById('testimonial-container');
            const scrollAmount = 350;
            container.scrollBy({
                left: direction * scrollAmount,
                behavior: 'smooth'
            });
        }

        // Simple animation on scroll
        const observerOptions = {
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.storage-card').forEach((card, index) => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(20px)';
            card.style.transition = `all 0.5s ease ${index * 0.1}s`;
            observer.observe(card);
        });
    </script>




</body></html>
