<!DOCTYPE html>

<html class="dark" lang="en" style=""><head><meta charset="utf-8"/><meta content="width=device-width, initial-scale=1.0" name="viewport"/><link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600;700&amp;family=Inter:wght@400;500;600;700&amp;display=swap" rel="stylesheet"/><link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/><style>@layer base{html,body{margin:0;padding:0;}body{overscroll-behavior:none;}main>:first-child{margin-top:0!important;}main>:last-child{margin-bottom:0!important;}}::-webkit-scrollbar{display:none;}@keyframes pulseGlow{0%,100%{opacity:1;filter:drop-shadow(0 0 6px #00FF66);}50%{opacity:0.4;filter:drop-shadow(0 0 2px #00FF66);}}.beacon-pulse{animation:pulseGlow 1.8s cubic-bezier(0.4,0,0.6,1) infinite;}
/* Toggle Switch Hardware Mechanism */
.toggle-baton {
  transition: transform 0.22s cubic-bezier(0.34, 1.56, 0.64, 1), box-shadow 0.2s ease;
}
.mode-schematic {
  filter: sepia(0.18) hue-rotate(185deg) contrast(1.08) brightness(1.1);
}
html.light-pcb {
  filter: invert(0.92) hue-rotate(180deg) contrast(1.05);
}
html.light-pcb img, html.light-pcb svg path {
  filter: invert(1) hue-rotate(180deg);
}
</style><script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script><script id="tailwind-config">tailwind.config={"darkMode":"class","theme":{"extend":{"colors":{"on-surface":"#e0e2ea","background":"#101419","secondary":"#ebffe6","on-secondary-fixed":"#002107","status-fault":"#FF3366","outline-variant":"#3a494b","secondary-fixed":"#6bff83","surface-dim":"#101419","primary":"#e0fdff","secondary-fixed-dim":"#00e55b","on-primary-container":"#006a70","tertiary-container":"#ffd3a8","trace-dim":"#30363D","on-error":"#690005","on-secondary-fixed-variant":"#00531b","on-tertiary":"#492900","tertiary-fixed":"#ffdcbc","error-container":"#93000a","surface-slot":"#161B22","on-secondary-container":"#007128","copper-foil":"#D97706","on-secondary":"#003911","on-tertiary-container":"#8b5200","on-error-container":"#ffdad6","secondary-container":"#00fe66","bus-cyan-dim":"#005662","tertiary-fixed-dim":"#ffb86b","on-tertiary-fixed":"#2c1700","on-surface-variant":"#b9cacb","surface-variant":"#31353b","primary-fixed":"#6ff6ff","primary-container":"#00f2fe","surface-container-low":"#181c21","primary-fixed-dim":"#00dce6","inverse-surface":"#e0e2ea","on-background":"#e0e2ea","surface-board":"#0D1117","surface":"#101419","status-active":"#00FF66","surface-container-high":"#262a30","surface-tint":"#00dce6","tertiary":"#fff6f0","on-primary":"#00373a","inverse-primary":"#00696f","status-standby":"#F59E0B","on-tertiary-fixed-variant":"#683d00","on-primary-fixed":"#002022","surface-bright":"#36393f","surface-raised":"#21262D","outline":"#849495","error":"#ffb4ab","silkscreen-bright":"#E6EDF3","inverse-on-surface":"#2d3136","on-primary-fixed-variant":"#004f53","surface-container":"#1c2025","silkscreen-subtle":"#8B949E","surface-container-highest":"#31353b","surface-container-lowest":"#0a0e14"},"borderRadius":{"DEFAULT":"0.25rem","lg":"0.5rem","xl":"0.75rem","full":"9999px"},"spacing":{"space-xxs":"0.125rem","space-2xl":"3rem","space-3xl":"4.5rem","gutter-desktop":"1.5rem","space-md":"1rem","margin-mobile":"1rem","space-lg":"1.5rem","trace-px":"1px","margin-desktop":"3rem","gutter-mobile":"1rem","space-sm":"0.5rem","space-xl":"2rem","space-xs":"0.25rem"},"fontFamily":{"label-micro":["JetBrains Mono"],"headline-sm":["JetBrains Mono"],"display-hero-mobile":["JetBrains Mono"],"label-caps":["JetBrains Mono"],"headline-lg-mobile":["JetBrains Mono"],"body-sm":["Inter"],"headline-md":["JetBrains Mono"],"display-hero":["JetBrains Mono"],"code-telemetry":["JetBrains Mono"],"headline-lg":["JetBrains Mono"],"body-lg":["Inter"],"body-md":["Inter"]},"fontSize":{"label-micro":["10px",{"lineHeight":"14px","letterSpacing":"0.1em","fontWeight":"500"}],"headline-sm":["16px",{"lineHeight":"24px","letterSpacing":"0.02em","fontWeight":"600"}],"display-hero-mobile":["32px",{"lineHeight":"40px","letterSpacing":"-0.01em","fontWeight":"700"}],"label-caps":["11px",{"lineHeight":"16px","letterSpacing":"0.08em","fontWeight":"600"}],"headline-lg-mobile":["24px",{"lineHeight":"32px","letterSpacing":"0em","fontWeight":"700"}],"body-sm":["12px",{"lineHeight":"18px","letterSpacing":"0.01em","fontWeight":"400"}],"headline-md":["20px",{"lineHeight":"28px","letterSpacing":"0em","fontWeight":"600"}],"display-hero":["48px",{"lineHeight":"56px","letterSpacing":"-0.02em","fontWeight":"700"}],"code-telemetry":["13px",{"lineHeight":"20px","letterSpacing":"0.02em","fontWeight":"500"}],"headline-lg":["32px",{"lineHeight":"40px","letterSpacing":"-0.01em","fontWeight":"700"}],"body-lg":["16px",{"lineHeight":"26px","letterSpacing":"0.01em","fontWeight":"400"}],"body-md":["14px",{"lineHeight":"22px","letterSpacing":"0em","fontWeight":"400"}]}}}};</script></head><body class="bg-surface-board font-body-md text-on-surface antialiased selection:bg-primary-container selection:text-on-primary-container min-h-screen flex flex-col"><header class="fixed top-0 w-full z-50 bg-surface-board/90 backdrop-blur-md shadow-[0_1px_8px_rgba(0,0,0,0.6)]"><div class="h-16 max-w-7xl mx-auto px-gutter-desktop flex items-center justify-between gap-space-md"><div class="flex items-center gap-space-md shrink-0"><div class="flex flex-col"><div class="flex items-center gap-space-xs"><span class="font-headline-sm text-headline-sm text-silkscreen-bright tracking-tight">&gt; AIDEN_</span><span class="font-label-caps text-label-caps text-primary bg-surface-slot px-space-xs py-space-xxs rounded">[SYS:ONLINE]</span></div><div class="flex items-center gap-space-xs"><span class="w-1.5 h-1.5 rounded-full bg-status-active beacon-pulse"></span><span class="font-label-micro text-label-micro text-silkscreen-subtle">24MHz SYS_CLK // STABLE</span></div></div></div><nav class="hidden xl:flex items-center gap-space-sm font-code-telemetry text-code-telemetry" data-active-classes="text-primary-container bg-surface-slot font-semibold"><a aria-current="page" class="px-space-sm py-space-xs rounded transition-colors text-primary-container bg-surface-slot font-semibold" data-path="portfolio" href="#">[01. Portfolio]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="store" href="#">[02. Store]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="open-source" href="#">[03. Open Source]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="contacto" href="#">[04. Contacto]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="links-and-redes" href="#">[Links &amp; Redes]</a></nav><div class="flex items-center gap-space-sm shrink-0"><!-- HARDWARE INDUSTRIAL SPDT THEME SWITCH --><div class="relative group flex items-center"><div class="bg-surface-slot/90 border border-trace-dim hover:border-primary/50 px-2 py-1 rounded flex items-center gap-2 shadow-inner select-none transition-colors"><div class="flex flex-col items-center gap-0.5"><div class="w-1.5 h-1.5 rounded-full bg-trace-dim/60 border border-silkscreen-subtle/40 flex items-center justify-center"><div class="w-0.5 h-0.5 bg-silkscreen-subtle/80 rounded-full"></div></div><span class="font-label-micro text-[8px] text-silkscreen-subtle leading-none tracking-tighter font-mono">SW1</span><div class="w-1.5 h-1.5 rounded-full bg-trace-dim/60 border border-silkscreen-subtle/40 flex items-center justify-center"><div class="w-0.5 h-0.5 bg-silkscreen-subtle/80 rounded-full"></div></div></div><div class="flex flex-col text-right leading-none"><span class="font-label-micro text-[8px] text-status-active font-mono font-bold tracking-tighter" id="sw-pos-dark">DARK</span><span class="font-label-micro text-[7px] text-silkscreen-subtle font-mono">NC</span></div><button aria-label="Toggle Theme: SPDT Hardware Switch" class="relative w-11 h-6 bg-surface-container-lowest rounded-full p-0.5 border border-trace-dim focus:outline-none focus:ring-1 focus:ring-primary-container shadow-[inset_0_1px_3px_rgba(0,0,0,0.8)] cursor-pointer" id="hardware-theme-switch" role="switch" title="SW_01 // THEME_SEL [DARK/LIGHT]"><div class="w-full h-full relative flex items-center justify-between px-1"><span class="font-mono text-[7px] text-status-active/80 font-semibold select-none">DK</span><span class="font-mono text-[7px] text-silkscreen-subtle/80 font-semibold select-none">UV</span></div><div class="toggle-baton absolute top-0.5 left-0.5 w-5 h-5 rounded-full bg-gradient-to-b from-[#b0b8c1] via-[#6e7681] to-[#30363d] border border-[#e6edf3]/40 shadow-[0_2px_4px_rgba(0,0,0,0.7),inset_0_1px_1px_rgba(255,255,255,0.7)] flex items-center justify-center" id="switch-lever"><div class="w-1.5 h-2 bg-gradient-to-b from-[#e6edf3] to-[#8b949e] rounded-sm shadow-[0_0_2px_rgba(0,0,0,0.5)]"></div></div></button><div class="flex flex-col text-left leading-none"><span class="font-label-micro text-[8px] text-silkscreen-subtle font-mono tracking-tighter" id="sw-pos-light">LIGHT</span><span class="font-label-micro text-[7px] text-silkscreen-subtle font-mono">NO</span></div><div class="flex items-center gap-1 pl-1 border-l border-trace-dim/60"><div class="relative flex items-center justify-center"><span class="w-2.5 h-2.5 rounded-full bg-status-active shadow-[0_0_8px_#00FF66] transition-all duration-300 border border-status-active/50" id="theme-led-indicator"></span></div><span class="font-label-micro text-[8px] text-silkscreen-bright font-mono font-bold" id="theme-status-lbl">PWR</span></div></div><!-- Serigraphed Technical Tooltip --><div class="absolute top-full mt-1.5 right-0 hidden group-hover:flex flex-col gap-0.5 bg-surface-slot text-silkscreen-bright border border-trace-dim p-1.5 rounded shadow-xl pointer-events-none z-50 whitespace-nowrap"><div class="flex items-center gap-1 font-label-micro text-[9px] text-primary-container font-mono"><span class="material-symbols-outlined text-[11px]">tune</span><span>SW_01 // THEME_SEL [DARK/LIGHT]</span></div><div class="text-[8px] text-silkscreen-subtle font-mono">SPDT HARDWARE LATCH // 3.3V LVTTL</div></div></div><a class="hidden sm:inline-flex items-center gap-space-xs px-space-sm py-space-xs font-code-telemetry text-code-telemetry text-silkscreen-bright bg-surface-slot hover:bg-surface-container-high hover:text-primary transition-all rounded" data-path="cv-hex" href="#"><span class="text-copper-foil font-bold">[↓]</span> CV.hex</a><a class="inline-flex items-center gap-space-xs px-space-md py-space-xs font-headline-sm text-headline-sm text-on-primary-fixed bg-primary-container hover:bg-secondary-fixed hover:text-on-secondary-fixed transition-all rounded shadow-[0_0_12px_rgba(0,242,254,0.35)]" data-path="store" href="#">[Tienda]</a><button aria-label="Open Hardware Telemetry Menu" class="xl:hidden p-space-xs rounded text-on-surface-variant hover:text-primary hover:bg-surface-container transition-colors" id="mobile-drawer-toggle"><span class="material-symbols-outlined text-[24px]">terminal</span></button></div></div><div class="hidden xl:hidden bg-surface-board shadow-xl" id="mobile-drawer"><div class="px-gutter-desktop py-space-md flex flex-col gap-space-xs font-code-telemetry text-code-telemetry"><div class="font-label-micro text-label-micro text-silkscreen-subtle px-space-xs py-space-xxs mb-space-xxs">&gt;&gt; HARDWARE_BUS_SELECT:</div><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="portfolio" href="#">[01. Portfolio]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="store" href="#">[02. Store]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="open-source" href="#">[03. Open Source]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="contacto" href="#">[04. Contacto]</a><a class="px-space-sm py-space-xs rounded text-on-surface-variant hover:text-on-surface hover:bg-surface-container-high transition-colors" data-path="links-and-redes" href="#">[Links &amp; Redes]</a><div class="pt-space-sm mt-space-xs flex items-center gap-space-sm"><a class="inline-flex items-center gap-space-xs px-space-sm py-space-xs font-code-telemetry text-code-telemetry text-silkscreen-bright bg-surface-slot hover:bg-surface-container-high hover:text-primary transition-all rounded" data-path="cv-hex" href="#"><span class="text-copper-foil font-bold">[↓]</span> CV.hex</a></div></div></div></header><main class="w-full flex-1 pt-16 bg-surface-board"><div class="flex flex-col w-full text-on-surface font-body-md selection:bg-primary-container selection:text-on-primary-container">
<!-- ========================================================================= -->
<!-- SECTION: SYSTEM TELEMETRY & HERO HEADER                                    -->
<!-- ========================================================================= -->
<section class="relative w-full overflow-hidden px-gutter-desktop py-space-xl lg:py-space-3xl max-w-7xl mx-auto">
<!-- Ambient Logic Grid Overlay (Decorative) -->
<div class="absolute inset-0 pointer-events-none opacity-20 bg-[radial-gradient(#30363D_1px,transparent_1px)] [background-size:24px_24px]"></div>
<!-- Hardware Trace Telemetry Strip -->
<div class="relative z-10 flex flex-wrap items-center justify-between gap-space-xs pb-space-md mb-space-lg border-b border-surface-raised font-label-micro text-label-micro text-silkscreen-subtle">
<div class="flex items-center gap-space-xs text-primary-container">
<span class="w-2 h-2 rounded-full bg-status-active beacon-pulse"></span>
<span class="">&gt; BOOT_SEQ_OK // UTN_FRBA_CORE v4.1 // SYS_CLK: 24.000 MHz // STATUS: READY</span>
</div>
<div class="hidden md:flex items-center gap-space-md">
<span class="text-silkscreen-bright">CORE_TEMP: 38.4°C</span>
<span class="text-copper-foil">BUS_V: 5.02V</span>
<span class="text-status-active">TX_RATE: 115200 BAUD</span>
</div>
</div>
<!-- Hero Content Layout: Split Cockpit -->
<div class="relative z-10 grid grid-cols-1 lg:grid-cols-12 gap-space-xl items-start">
<!-- Left 8 Cols: Main Identity & Bio -->
<div class="lg:col-span-8 flex flex-col gap-space-md">
<div class="inline-flex items-center gap-space-xs font-code-telemetry text-code-telemetry text-primary-container">
<span class="font-bold">&gt;</span>
<span class="tracking-widest uppercase">Inicializando sistema...</span>
<span class="inline-block w-2 h-4 bg-primary-container animate-pulse ml-space-xxs"></span>
</div>
<h1 class="font-display-hero text-display-hero text-silkscreen-bright tracking-tight leading-tight">
          Hola, soy <span class="text-primary-container drop-shadow-[0_0_16px_rgba(0,242,254,0.4)]">Aiden</span>.
        </h1>
<div class="flex items-center gap-space-sm font-headline-lg text-headline-lg text-on-surface-variant">
<span class="text-copper-foil font-bold">#</span>
<h2 class="">Diseñador de Hardware &amp; Software.</h2>
</div>
<p class="font-body-lg text-body-lg text-on-surface-variant max-w-2xl leading-relaxed mt-space-xs">
          Estudiante de Ingeniería Electrónica en UTN e instructor de robótica. Especializado en electrónica DIY, diseño de PCBs y sistemas embebidos. Transformo esquemáticos en realidades físicas, desde la mesa de dibujo hasta la línea de ensamblaje.
        </p>
<!-- Hardware Tags Spec Bar -->
<div class="flex flex-wrap gap-space-xs mt-space-sm font-label-caps text-label-caps">
<span class="px-space-sm py-space-xxs rounded bg-surface-slot text-primary border border-trace-dim">[PWR: 3.3V/5V]</span>
<span class="px-space-sm py-space-xxs rounded bg-surface-slot text-secondary-fixed border border-trace-dim">[KiCad Pro]</span>
<span class="px-space-sm py-space-xxs rounded bg-surface-slot text-silkscreen-bright border border-trace-dim">[Firmware C/C++]</span>
<span class="px-space-sm py-space-xxs rounded bg-surface-slot text-tertiary-container border border-trace-dim">[SMD 0603]</span>
<span class="px-space-sm py-space-xxs rounded bg-surface-slot text-primary-fixed border border-trace-dim">[STM32 / ESP32]</span>
</div>
<!-- Cybernetic Action Buttons -->
<div class="flex flex-wrap items-center gap-space-sm mt-space-lg">
<a class="px-space-md py-space-sm rounded bg-primary-container text-on-primary-fixed font-headline-sm text-headline-sm hover:bg-secondary-fixed hover:text-on-secondary-fixed transition-all shadow-[0_0_16px_rgba(0,242,254,0.35)] flex items-center gap-space-xs" href="#">
<span class="font-bold">[↓]</span> Descargar CV
          </a>
<a class="px-space-md py-space-sm rounded bg-surface-slot text-silkscreen-bright font-headline-sm text-headline-sm hover:text-primary-container hover:bg-surface-container-high transition-all flex items-center gap-space-xs border border-trace-dim" href="#store">
<span class="">Ir a la Tienda</span> <span class="text-copper-foil">→</span>
</a>
<a class="px-space-md py-space-sm rounded bg-surface-slot text-copper-foil font-headline-sm text-headline-sm hover:bg-surface-container-high transition-all flex items-center gap-space-xs border border-trace-dim" href="#contacto">
<span class="">Contactarse</span>
</a>
</div>
</div>
<!-- Right 4 Cols: Oscilloscope Logic Telemetry Bay -->
<div class="lg:col-span-4 w-full bg-surface-slot p-space-md rounded-lg border border-surface-raised shadow-xl flex flex-col gap-space-sm">
<div class="flex items-center justify-between border-b border-surface-raised pb-space-xs font-label-micro text-label-micro">
<span class="text-silkscreen-subtle uppercase tracking-wider">&gt;&gt; SCOPE_CH1: PWM_OUT</span>
<span class="text-status-active flex items-center gap-space-xxs">
<span class="w-1.5 h-1.5 rounded-full bg-status-active beacon-pulse"></span> TRIG'D
          </span>
</div>
<!-- Oscilloscope Waveform Display (Inline SVG Under 2KB) -->
<div class="w-full h-28 bg-surface-container-lowest rounded relative overflow-hidden flex items-center justify-center p-space-xs">
<!-- Background Grid Lines -->
<div class="absolute inset-0 bg-[linear-gradient(to_right,#161B22_1px,transparent_1px),linear-gradient(to_bottom,#161B22_1px,transparent_1px)] bg-[size:16px_16px] opacity-40"></div>
<!-- Waveform SVG Line -->
<svg class="w-full h-full text-status-active relative z-10" fill="none" preserveaspectratio="none" viewbox="0 0 320 80">
<path class="drop-shadow-[0_0_6px_#00FF66]" d="M0,40 L30,40 L30,12 L70,12 L70,68 L110,68 L110,12 L150,12 L150,68 L190,68 L190,12 L230,12 L230,68 L270,68 L270,40 L320,40" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"></path>
<circle class="beacon-pulse" cx="110" cy="12" fill="#00FF66" r="3"></circle>
<circle class="beacon-pulse" cx="230" cy="68" fill="#00FF66" r="3"></circle>
</svg>
</div>
<!-- Telemetry Data Matrix -->
<div class="grid grid-cols-2 gap-space-xs font-label-micro text-label-micro">
<div class="p-space-xs rounded bg-surface-container flex flex-col">
<span class="text-silkscreen-subtle">V_PEAK:</span>
<span class="text-silkscreen-bright font-code-telemetry">12.44 V</span>
</div>
<div class="p-space-xs rounded bg-surface-container flex flex-col">
<span class="text-silkscreen-subtle">FREQ:</span>
<span class="text-primary-container font-code-telemetry">20.0 kHz</span>
</div>
<div class="p-space-xs rounded bg-surface-container flex flex-col">
<span class="text-silkscreen-subtle">DUTY_CYCLE:</span>
<span class="text-secondary-fixed font-code-telemetry">72.6 %</span>
</div>
<div class="p-space-xs rounded bg-surface-container flex flex-col">
<span class="text-silkscreen-subtle">JITTER:</span>
<span class="text-copper-foil font-code-telemetry">&lt; 14 ns</span>
</div>
</div>
<!-- Logic Pinout Mini Diagnostic -->
<div class="flex flex-col gap-space-xxs border border-trace-dim rounded bg-surface-container-lowest overflow-hidden mt-space-xs font-label-micro text-label-micro"><div class="bg-surface-container px-space-xs py-space-xxs flex items-center justify-between border-b border-trace-dim"><span class="text-primary-container font-bold tracking-wider uppercase font-code-telemetry">ABSOLUTE MAXIMUM ratings</span><span class="text-silkscreen-subtle text-[10px]">DS_REV: 4.1</span></div><div class="overflow-x-auto"><table class="w-full text-left border-collapse"><thead class="bg-surface-slot text-silkscreen-subtle border-b border-trace-dim font-label-caps text-[10px]"><tr><th class="py-space-xxs px-space-xs text-silkscreen-subtle font-semibold">PARAMETER</th><th class="py-space-xxs px-space-xs text-primary-container font-semibold">SPECIFICATION / RATING</th><th class="py-space-xxs px-space-xs text-silkscreen-subtle font-semibold text-right">UNIT / NOTES</th></tr></thead><tbody class="divide-y divide-trace-dim font-code-telemetry text-[11px]"><tr class="hover:bg-surface-slot/60 transition-colors"><td class="py-space-xxs px-space-xs text-silkscreen-subtle">DISCIPLINA</td><td class="py-space-xxs px-space-xs text-silkscreen-bright font-medium">Hardware &amp; Embedded Firmware / Robotics</td><td class="py-space-xxs px-space-xs text-copper-foil text-right">SYS_CORE</td></tr><tr class="hover:bg-surface-slot/60 transition-colors"><td class="py-space-xxs px-space-xs text-silkscreen-subtle">EDA_SUITE</td><td class="py-space-xxs px-space-xs text-silkscreen-bright">KiCad Pro v8 / Altium</td><td class="py-space-xxs px-space-xs text-silkscreen-subtle text-right">CAD / CAM</td></tr><tr class="hover:bg-surface-slot/60 transition-colors"><td class="py-space-xxs px-space-xs text-silkscreen-subtle">MCU_ARCH</td><td class="py-space-xxs px-space-xs text-primary font-medium">STM32F4 / RP2040 / ESP32</td><td class="py-space-xxs px-space-xs text-silkscreen-subtle text-right">ARM / RISC-V</td></tr><tr class="hover:bg-surface-slot/60 transition-colors"><td class="py-space-xxs px-space-xs text-silkscreen-subtle">LANGUAGES</td><td class="py-space-xxs px-space-xs text-silkscreen-bright">C / C++20 / Rust / Python</td><td class="py-space-xxs px-space-xs text-silkscreen-subtle text-right">NATIVE_LL</td></tr><tr class="hover:bg-surface-slot/60 transition-colors"><td class="py-space-xxs px-space-xs text-silkscreen-subtle">UBICACIÓN</td><td class="py-space-xxs px-space-xs text-silkscreen-bright">CABA, Argentina (UTN FRBA)</td><td class="py-space-xxs px-space-xs text-silkscreen-subtle text-right">UTC-3</td></tr><tr class="hover:bg-surface-slot/60 transition-colors"><td class="py-space-xxs px-space-xs text-silkscreen-subtle">ESTADO</td><td class="py-space-xxs px-space-xs"><span class="inline-flex items-center gap-space-xxs text-status-active font-semibold"><span class="w-1.5 h-1.5 rounded-full bg-status-active beacon-pulse"></span>DISPONIBLE (ACTIVE)</span></td><td class="py-space-xxs px-space-xs text-status-active text-right font-medium">LOW LATENCY</td></tr></tbody></table></div></div><div class="pt-space-xs border-t border-surface-raised flex items-center justify-between font-label-micro text-label-micro text-silkscreen-subtle">
<span class="">PIN_MODE: PUSH_PULL</span>
<span class="text-primary font-bold">STM32F401RE</span>
</div>
</div>
</div>
</section>
<!-- ========================================================================= -->
<!-- SECTION 01: PORTFOLIO                                                     -->
<!-- ========================================================================= -->
<section class="w-full bg-surface-container-low py-space-2xl border-t border-b border-surface-raised" id="portfolio">
<div class="max-w-7xl mx-auto px-gutter-desktop flex flex-col gap-space-xl">
<!-- Section Header -->
<div class="flex items-center justify-between gap-space-md border-b border-trace-dim pb-space-sm">
<div class="flex items-center gap-space-sm">
<span class="font-headline-lg text-headline-lg text-primary-container font-bold">01.</span>
<h2 class="font-headline-lg text-headline-lg text-silkscreen-bright">Portfolio</h2>
</div>
<!-- Pagination / Carousel Controls -->
<div class="flex items-center gap-space-xs">
<button class="w-8 h-8 rounded bg-surface-slot border border-trace-dim text-silkscreen-bright flex items-center justify-center hover:text-primary hover:border-primary-container transition-all">
<span class="material-symbols-outlined text-sm">chevron_left</span>
</button>
<button class="w-8 h-8 rounded bg-surface-slot border border-trace-dim text-silkscreen-bright flex items-center justify-center hover:text-primary hover:border-primary-container transition-all">
<span class="material-symbols-outlined text-sm">chevron_right</span>
</button>
</div>
</div>
<!-- Project Matrix Grid -->
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-space-lg">
<!-- Project 1: AT0M -->
<article class="bg-surface-slot rounded-lg border border-surface-raised overflow-hidden flex flex-col group hover:border-primary-container transition-all duration-300 shadow-lg">
<div class="relative aspect-[4/3] w-full overflow-hidden bg-surface-board">
<img alt="Autonomous battle sumo robot project AT0M, titanium wedge chassis, brushless motors, custom PCB exposed" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDxt-3-lhZEWuRxhqNfZU4Bb2zYfFMyANtkaPWPJH5KTuaPEymk47toN1D6MpKs7OP-QYavc8UWVq2ncjLwCWtEXhO6NrQ96dz7ukdHC1PXCgRvXWo_Seehyy35S6eW6e2dEgUl7aWZmN16iUmSkBBtXASRr0YN90YZ1CWRC5xHOEFCbXUGZSBhp0iLTiBD3TGw0iK7tOMHBQ2UZF13SlAAbYXSWJgvLmKxurztt8y2YMUmoClvskpJQQ"/>
<div class="absolute top-space-xs left-space-xs px-space-xs py-space-xxs rounded bg-surface-board/90 backdrop-blur font-label-micro text-label-micro text-secondary-fixed border border-secondary-fixed/40 flex items-center gap-space-xxs">
<span class="w-1.5 h-1.5 rounded-full bg-status-active"></span> HARDWARE READY
            </div>
</div>
<div class="p-space-md flex flex-col flex-1 justify-between gap-space-md">
<div class="flex flex-col gap-space-xs">
<span class="font-label-micro text-label-micro text-copper-foil">SYS_ID: U01_ROBOT_SUMO</span>
<h3 class="font-headline-md text-headline-md text-silkscreen-bright">Proyecto AT0M</h3>
<p class="font-body-md text-body-md text-on-surface-variant">
                Diseño integral de robot sumo autónomo de competencia.
              </p>
<div class="flex flex-wrap gap-space-xxs mt-space-xs font-label-micro text-label-micro">
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-silkscreen-bright border border-trace-dim">[Autonomous]</span>
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-primary-container border border-trace-dim">[Brushless]</span>
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-secondary-fixed border border-trace-dim">[Custom PCB]</span>
</div>
</div>
<a class="w-full py-space-xs rounded bg-surface-container-high text-silkscreen-bright font-code-telemetry text-code-telemetry text-center hover:bg-primary-container hover:text-on-primary-fixed transition-all border border-trace-dim" href="#">
              Ver DevBlog
            </a>
</div>
</article>
<!-- Project 2: Docente de Robótica -->
<article class="bg-surface-slot rounded-lg border border-surface-raised overflow-hidden flex flex-col group hover:border-primary-container transition-all duration-300 shadow-lg">
<div class="relative aspect-[4/3] w-full overflow-hidden bg-surface-board p-space-lg flex flex-col justify-center items-center">
<!-- Procedural Educational Schematic Graphic -->
<div class="w-full h-full rounded bg-surface-container-lowest border border-trace-dim p-space-md flex flex-col justify-between relative overflow-hidden">
<div class="flex items-center justify-between font-label-micro text-label-micro text-silkscreen-subtle">
<span class="">WORKBENCH_EDU // 02</span>
<span class="text-copper-foil">UTN_FRBA</span>
</div>
<div class="flex flex-col items-center justify-center gap-space-xs">
<span class="material-symbols-outlined text-primary-container text-4xl">precision_manufacturing</span>
<span class="font-code-telemetry text-code-telemetry text-silkscreen-bright font-semibold">Cultura Maker &amp; Prototipado</span>
</div>
<div class="h-1 w-full bg-surface-raised rounded-full overflow-hidden">
<div class="h-full bg-primary-container w-3/4"></div>
</div>
</div>
<div class="absolute top-space-xs left-space-xs px-space-xs py-space-xxs rounded bg-surface-board/90 backdrop-blur font-label-micro text-label-micro text-primary border border-primary/40 flex items-center gap-space-xxs">
<span class="w-1.5 h-1.5 rounded-full bg-status-active"></span> ACTIVE MENTOR
            </div>
</div>
<div class="p-space-md flex flex-col flex-1 justify-between gap-space-md">
<div class="flex flex-col gap-space-xs">
<span class="font-label-micro text-label-micro text-copper-foil">SYS_ID: EDU_CURRICULA</span>
<h3 class="font-headline-md text-headline-md text-silkscreen-bright">Docente de Robótica</h3>
<p class="font-body-md text-body-md text-on-surface-variant">
                Diseño de currícula enfocada en cultura Maker.
              </p>
<div class="flex flex-wrap gap-space-xxs mt-space-xs font-label-micro text-label-micro">
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-silkscreen-bright border border-trace-dim">[Maker Culture]</span>
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-primary-container border border-trace-dim">[Hardware Edu]</span>
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-copper-foil border border-trace-dim">[3D Printing]</span>
</div>
</div>
<a class="w-full py-space-xs rounded bg-surface-container-high text-silkscreen-bright font-code-telemetry text-code-telemetry text-center hover:bg-primary-container hover:text-on-primary-fixed transition-all border border-trace-dim" href="#">
              Ver Más
            </a>
</div>
</article>
<!-- Project 3: RBK7FTC - Mentoreo -->
<article class="bg-surface-slot rounded-lg border border-surface-raised overflow-hidden flex flex-col group hover:border-primary-container transition-all duration-300 shadow-lg">
<div class="relative aspect-[4/3] w-full overflow-hidden bg-surface-board">
<img alt="FIRST Tech Challenge competition robot RBK7FTC, anodized aluminum structural channels, omni wheels, wire harness" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" src="https://lh3.googleusercontent.com/aida-public/AB6AXuAxg7GTFiUCB5UvojVg6octGf8weZADriYCscpRamxplxf6t2PKpc5F3O5YcgfM3aato2y1gNHZFlgp655Slc8A8ko76xMrktWh_r825x6hlj-6e5dUwvnR6NVZUpPXhGDm9qf_nTs0zk4VdDelhoQwUli15C5mThJFJJB_KEGfmHDfzOo_dByY3JZRh5WUqKxhJPZazMaGrdaDKs2JiAn9h5waIA1GGIKuqAtMowl8weg0wbw6ujS1cA"/>
<div class="absolute top-space-xs left-space-xs px-space-xs py-space-xxs rounded bg-surface-board/90 backdrop-blur font-label-micro text-label-micro text-copper-foil border border-copper-foil/40 flex items-center gap-space-xxs">
<span class="w-1.5 h-1.5 rounded-full bg-status-standby"></span> INTL_QUALIFIED
            </div>
</div>
<div class="p-space-md flex flex-col flex-1 justify-between gap-space-md">
<div class="flex flex-col gap-space-xs">
<span class="font-label-micro text-label-micro text-copper-foil">SYS_ID: FTC_COMPETITION</span>
<h3 class="font-headline-md text-headline-md text-silkscreen-bright">RBK7FTC - Mentoreo</h3>
<p class="font-body-md text-body-md text-on-surface-variant">
                6to puesto y clasificación internacional a México. Optimización técnica para alto rendimiento.
              </p>
<div class="flex flex-wrap gap-space-xxs mt-space-xs font-label-micro text-label-micro">
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-silkscreen-bright border border-trace-dim">[FIRST Tech Challenge]</span>
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-primary-container border border-trace-dim">[Robotics]</span>
<span class="px-space-xs py-space-xxs bg-surface-container rounded text-secondary-fixed border border-trace-dim">[Telemetry]</span>
</div>
</div>
<a class="w-full py-space-xs rounded bg-surface-container-high text-silkscreen-bright font-code-telemetry text-code-telemetry text-center hover:bg-primary-container hover:text-on-primary-fixed transition-all border border-trace-dim" href="#">
              Ver DevBlog
            </a>
</div>
</article>
</div>
<!-- Action Footer: Explore All -->
<div class="flex justify-center pt-space-md">
<a class="px-space-xl py-space-sm rounded bg-surface-container-high text-silkscreen-bright font-headline-sm text-headline-sm hover:bg-secondary-container hover:text-on-secondary-container transition-all border border-trace-dim shadow-md flex items-center gap-space-xs" href="#">
<span class="">[Explorar todo el Portfolio]</span>
</a>
</div>
</div>
</section>
<!-- ========================================================================= -->
<!-- SECTION 02: STORE                                                         -->
<!-- ========================================================================= -->
<section class="w-full py-space-2xl max-w-7xl mx-auto px-gutter-desktop" id="store">
<div class="flex flex-col gap-space-xl">
<!-- Header -->
<div class="flex items-center justify-between border-b border-trace-dim pb-space-sm">
<div class="flex items-center gap-space-sm">
<span class="font-headline-lg text-headline-lg text-primary-container font-bold">02.</span>
<h2 class="font-headline-lg text-headline-lg text-silkscreen-bright">Store</h2>
</div>
<span class="font-label-caps text-label-caps text-copper-foil bg-surface-slot px-space-sm py-space-xxs rounded border border-trace-dim">
          HARDWARE_LAB_BATCH_01
        </span>
</div>
<!-- Store Showcase Card -->
<div class="bg-surface-slot rounded-xl border border-surface-raised p-space-lg lg:p-space-xl grid grid-cols-1 lg:grid-cols-12 gap-space-xl items-center shadow-2xl relative overflow-hidden">
<!-- Glow Backdrop -->
<div class="absolute -right-20 -top-20 w-80 h-80 bg-primary-container/5 rounded-full blur-3xl pointer-events-none"></div>
<!-- Product PCB Image Bay -->
<div class="lg:col-span-6 relative rounded-lg overflow-hidden border border-trace-dim bg-surface-board">
<img alt="Custom TitanCore 7960 high-power motor driver PCB board, dual MOSFETs, heavy copper traces, screw terminals, heat sink" class="w-full aspect-[4/3] object-cover" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDCWgyYwS6tJtY5u6_tq6wQTNMFWpupWc4Gc-eMrYs-4VHVRwanTsej9mrnizAZXKx1ZeBKxgZ-aiRzateXSPTinwv_f-sIHivFqGtIfmKIafECB-wQBiHf5BB_puaVcLI5FRCDIhZIEHiRGqWAOUrp2y02kXhjxDEb62zO45FKG1zZJGHMd-5qnxJx35gxUGG8YYN8ZYsCEvZlTNWXSfsRbRUTcOjVkXfyFwRAOYnvkM04OBCmIf2SRQ"/>
<div class="absolute top-space-sm right-space-sm">
<span class="px-space-sm py-space-xs rounded bg-status-active/20 text-status-active border border-status-active font-headline-sm text-headline-sm font-bold tracking-wider backdrop-blur-md">
              COMING SOON
            </span>
</div>
</div>
<!-- Product Specs & Command Module -->
<div class="lg:col-span-6 flex flex-col gap-space-md">
<div class="flex items-center justify-between">
<span class="font-label-micro text-label-micro text-silkscreen-subtle">SKU: TC-7960-PRO</span>
<span class="font-label-caps text-label-caps text-status-active flex items-center gap-space-xxs">
<span class="w-1.5 h-1.5 rounded-full bg-status-active"></span> IN FABRICATION
            </span>
</div>
<h3 class="font-display-hero-mobile text-display-hero-mobile text-silkscreen-bright font-bold">
            TitanCore 7960
          </h3>
<div class="flex items-baseline gap-space-xs">
<span class="font-headline-lg text-headline-lg text-primary-container font-bold">USD 28.00</span>
<span class="font-label-micro text-label-micro text-silkscreen-subtle">(Pre-order price / Free shipping CABA)</span>
</div>
<p class="font-body-md text-body-md text-on-surface-variant leading-relaxed">
            Módulo driver puente H de alta potencia diseñado para soportar exigencias de combate y robótica móvil extrema. Optimización de pistas de cobre 2oz y disipador térmico de aluminio mecanizado CNC.
          </p>
<!-- Hardware Quick Specs Table -->
<div class="grid grid-cols-2 sm:grid-cols-4 gap-space-xs font-label-micro text-label-micro">
<div class="p-space-xs rounded bg-surface-container border border-trace-dim flex flex-col">
<span class="text-silkscreen-subtle">VOLTAGE</span>
<span class="text-silkscreen-bright font-bold">5.5V - 27V</span>
</div>
<div class="p-space-xs rounded bg-surface-container border border-trace-dim flex flex-col">
<span class="text-silkscreen-subtle">CURRENT</span>
<span class="text-copper-foil font-bold">43A Peak</span>
</div>
<div class="p-space-xs rounded bg-surface-container border border-trace-dim flex flex-col">
<span class="text-silkscreen-subtle">PWM FREQ</span>
<span class="text-primary font-bold">Up to 25kHz</span>
</div>
<div class="p-space-xs rounded bg-surface-container border border-trace-dim flex flex-col">
<span class="text-silkscreen-subtle">PROTECTION</span>
<span class="text-status-active font-bold">Thermal/OCP</span>
</div>
</div>
<div class="pt-space-sm flex flex-wrap items-center gap-space-sm">
<button class="px-space-md py-space-sm rounded bg-surface-container-high text-silkscreen-subtle font-code-telemetry text-code-telemetry cursor-not-allowed border border-trace-dim flex items-center gap-space-xs" disabled="">
<span class="material-symbols-outlined text-sm">lock</span> [Reservas Próximamente]
            </button>
<a class="px-space-md py-space-sm rounded bg-surface-slot text-silkscreen-bright font-code-telemetry text-code-telemetry hover:text-primary transition-all border border-trace-dim" href="#contacto">
              Consultar Disponibilidad Batch →
            </a>
</div>
</div>
</div>
</div>
</section>
<!-- ========================================================================= -->
<!-- SECTION 03: OPEN SOURCE                                                   -->
<!-- ========================================================================= -->
<section class="w-full bg-surface-container-low py-space-2xl border-t border-b border-surface-raised" id="opensource">
<div class="max-w-7xl mx-auto px-gutter-desktop flex flex-col gap-space-xl">
<!-- Header -->
<div class="flex items-center justify-between border-b border-trace-dim pb-space-sm">
<div class="flex items-center gap-space-sm">
<span class="font-headline-lg text-headline-lg text-primary-container font-bold">03.</span>
<h2 class="font-headline-lg text-headline-lg text-silkscreen-bright">Open Source</h2>
</div>
<span class="font-label-caps text-label-caps text-status-active flex items-center gap-space-xxs">
<span class="material-symbols-outlined text-sm">code</span> LICENCIA LIBRE
        </span>
</div>
<!-- Main Open Source Component Unit -->
<div class="bg-surface-slot rounded-lg border border-surface-raised p-space-lg flex flex-col gap-space-md">
<div class="flex flex-col md:flex-row md:items-center justify-between gap-space-sm">
<div class="flex flex-col gap-space-xxs">
<span class="font-label-micro text-label-micro text-copper-foil">&gt; HARDWARE_REPO // REV_1.2</span>
<h3 class="font-headline-lg text-headline-lg text-silkscreen-bright font-bold">
              TitanCore-7960 - Driver de Motores
            </h3>
</div>
<div class="flex flex-wrap gap-space-xs">
<span class="px-space-sm py-space-xxs rounded bg-surface-container text-primary border border-trace-dim font-label-caps text-label-caps">
              KiCad Hardware
            </span>
<span class="px-space-sm py-space-xxs rounded bg-surface-container text-secondary-fixed border border-trace-dim font-label-caps text-label-caps">
              GPL v3.0
            </span>
<span class="px-space-sm py-space-xxs rounded bg-surface-container text-silkscreen-subtle border border-trace-dim font-label-caps text-label-caps">
              Gerbers Ready
            </span>
</div>
</div>
<p class="font-body-lg text-body-lg text-on-surface-variant max-w-3xl leading-relaxed">
          Diseño de driver open source para robots de combate. Incluye archivos esquemáticos de KiCad, layout de PCB en 2 capas, listado BOM de componentes SMD comerciales y curvas de testeo térmico.
        </p>
<!-- Command Controls Row -->
<div class="flex flex-wrap items-center gap-space-sm pt-space-xs">
<a class="px-space-md py-space-xs rounded bg-surface-container-high text-silkscreen-bright font-code-telemetry text-code-telemetry hover:bg-primary-container hover:text-on-primary-fixed transition-all border border-trace-dim flex items-center gap-space-xs" href="https://github.com/Aid-Code" rel="noopener noreferrer" target="_blank">
<span class="material-symbols-outlined text-sm">terminal</span> GitHub
          </a>
<a class="px-space-md py-space-xs rounded bg-primary-container text-on-primary-fixed font-code-telemetry text-code-telemetry hover:bg-secondary-fixed hover:text-on-secondary-fixed transition-all font-semibold flex items-center gap-space-xs" href="#">
<span class="material-symbols-outlined text-sm">menu_book</span> Ver DevBlog
          </a>
</div>
</div>
<!-- Action Footer -->
<div class="flex justify-center">
<a class="px-space-lg py-space-sm rounded bg-surface-slot text-on-surface-variant font-code-telemetry text-code-telemetry hover:text-silkscreen-bright hover:bg-surface-container-high transition-all border border-trace-dim" href="#">
          [Ver Todas las Contribuciones]
        </a>
</div>
</div>
</section>
<!-- ========================================================================= -->
<!-- SECTION 04: CONTACTO                                                      -->
<!-- ========================================================================= -->
<section class="w-full py-space-2xl max-w-7xl mx-auto px-gutter-desktop" id="contacto">
<div class="flex flex-col gap-space-xl">
<!-- Header -->
<div class="flex items-center justify-between border-b border-trace-dim pb-space-sm">
<div class="flex items-center gap-space-sm">
<span class="font-headline-lg text-headline-lg text-primary-container font-bold">04.</span>
<h2 class="font-headline-lg text-headline-lg text-silkscreen-bright">Contacto</h2>
</div>
<span class="font-label-micro text-label-micro text-silkscreen-subtle">CHANNEL: DIRECT_IO</span>
</div>
<!-- Terminal Transmission Form Bay -->
<div class="max-w-3xl mx-auto w-full bg-surface-slot rounded-xl border border-surface-raised p-space-lg lg:p-space-xl flex flex-col gap-space-lg shadow-2xl">
<div class="flex flex-col gap-space-xs">
<p class="font-body-lg text-body-lg text-silkscreen-bright">
            Completá el formulario para consultas sobre desarrollos de hardware, clases o colaboraciones.
          </p>
<span class="font-label-micro text-label-micro text-copper-foil">&gt; BUFFER_STATUS: AWAITING_INPUT</span>
</div>
<form class="flex flex-col gap-space-md" onsubmit="event.preventDefault(); alert('[TX_SUCCESS]: Mensaje transmitido al bus.');">
<!-- Field: Alias -->
<div class="flex flex-col gap-space-xxs">
<label class="font-label-caps text-label-caps text-on-surface-variant flex items-center gap-space-xxs" for="alias-input">
<span class="text-primary-container">&gt;_</span> Nombre / Alias:
            </label>
<input class="w-full bg-surface-board rounded px-space-md py-space-sm border border-trace-dim text-silkscreen-bright font-code-telemetry text-code-telemetry focus:outline-none focus:border-primary-container focus:ring-1 focus:ring-primary-container transition-all" id="alias-input" placeholder="p. ej. Ing. Martinez" required="" type="text"/>
</div>
<!-- Field: Email -->
<div class="flex flex-col gap-space-xxs">
<label class="font-label-caps text-label-caps text-on-surface-variant flex items-center gap-space-xxs" for="email-input">
<span class="text-primary-container">&gt;_</span> Email:
            </label>
<input class="w-full bg-surface-board rounded px-space-md py-space-sm border border-trace-dim text-silkscreen-bright font-code-telemetry text-code-telemetry focus:outline-none focus:border-primary-container focus:ring-1 focus:ring-primary-container transition-all" id="email-input" placeholder="nombre@laboratorio.com" required="" type="email"/>
</div>
<!-- Field: Message Payload -->
<div class="flex flex-col gap-space-xxs">
<label class="font-label-caps text-label-caps text-on-surface-variant flex items-center gap-space-xxs" for="payload-input">
<span class="text-primary-container">&gt;_</span> Mensaje de transmisión...:
            </label>
<textarea class="w-full bg-surface-board rounded px-space-md py-space-sm border border-trace-dim text-silkscreen-bright font-code-telemetry text-code-telemetry focus:outline-none focus:border-primary-container focus:ring-1 focus:ring-primary-container transition-all resize-none" id="payload-input" placeholder="Detalles sobre el esquemático, robot o proyecto pedagógico..." required="" rows="4"></textarea>
</div>
<!-- Submit Button -->
<button class="mt-space-xs w-full py-space-sm rounded bg-primary-container text-on-primary-fixed font-headline-sm text-headline-sm font-bold tracking-wide hover:bg-secondary-fixed hover:text-on-secondary-fixed transition-all shadow-[0_0_16px_rgba(0,242,254,0.3)] flex items-center justify-center gap-space-xs" type="submit">
<span class="">[&gt;] Enviar Mensaje</span>
</button>
</form>
</div>
</div>
</section>
<!-- ========================================================================= -->
<!-- SECTION: LINKS & REDES HUB                                                -->
<!-- ========================================================================= -->
<section class="w-full py-space-xl bg-surface-container-low border-t border-surface-raised">
<div class="max-w-4xl mx-auto px-gutter-desktop text-center flex flex-col items-center gap-space-md">
<div class="flex items-center gap-space-xs font-label-micro text-label-micro text-primary-container">
<span class="w-2 h-2 rounded-full bg-status-active"></span>
<span class="">NODE_ID: DIRECTORY_HUB</span>
</div>
<h2 class="font-headline-lg text-headline-lg text-silkscreen-bright font-bold">
        Links &amp; Redes
      </h2>
<p class="font-body-lg text-body-lg text-on-surface-variant max-w-xl">
        Explorá mi contenido, repositorios y redes sociales en un solo lugar.
      </p>
<a class="px-space-xl py-space-sm rounded bg-surface-slot text-primary-container font-headline-sm text-headline-sm border border-primary-container hover:bg-primary-container hover:text-on-primary-fixed transition-all shadow-[0_0_12px_rgba(0,242,254,0.2)]" href="#">
        Ver Links &amp; Redes
      </a>
</div>
</section>
</div></main><footer class="w-full bg-surface-container-lowest"><div class="max-w-7xl mx-auto px-gutter-desktop py-space-lg flex flex-col md:flex-row items-center justify-between gap-space-md"><div class="flex flex-wrap items-center gap-x-space-sm gap-y-space-xxs font-label-micro text-label-micro text-silkscreen-subtle"><span class="text-silkscreen-bright">© 2026 AIDEN</span><span class="">//</span><span class="text-primary">PCB Rev 2.4</span><span class="">//</span><span class="">Ensamblado a mano en CABA</span><span class="">//</span><span class="">UTN FRBA Electronics</span></div><div class="flex items-center gap-space-md font-code-telemetry text-code-telemetry"><div class="flex items-center gap-space-xs text-status-active"><span class="w-2 h-2 rounded-full bg-status-active beacon-pulse"></span><span class="font-label-caps text-label-caps">BUS: 3.3V LVTTL</span></div><span class="font-label-micro text-label-micro text-silkscreen-subtle bg-surface-slot px-space-xs py-space-xxs rounded">Latency: 4ms</span></div></div></footer><script>const toggleBtn=document.getElementById('mobile-drawer-toggle');const drawer=document.getElementById('mobile-drawer');if(toggleBtn&&drawer){toggleBtn.addEventListener('click',()=>{drawer.classList.toggle('hidden');});}

// Industrial SPDT Hardware Toggle Switch Logic
const themeSwitch = document.getElementById('hardware-theme-switch');
const switchLever = document.getElementById('switch-lever');
const ledIndicator = document.getElementById('theme-led-indicator');
const posDark = document.getElementById('sw-pos-dark');
const posLight = document.getElementById('sw-pos-light');
const statusLbl = document.getElementById('theme-status-lbl');
let isLightMode = false;

if(themeSwitch && switchLever && ledIndicator) {
  themeSwitch.addEventListener('click', () => {
    isLightMode = !isLightMode;
    if(isLightMode) {
      // Actuate switch to RIGHT (UV / Light Clean PCB)
      switchLever.style.transform = 'translateX(20px)';
      ledIndicator.className = 'w-2.5 h-2.5 rounded-full bg-status-standby shadow-[0_0_8px_#F59E0B] transition-all duration-300 border border-status-standby/50';
      if(posDark) { posDark.className = 'font-label-micro text-[8px] text-silkscreen-subtle font-mono'; }
      if(posLight) { posLight.className = 'font-label-micro text-[8px] text-status-standby font-mono font-bold tracking-tighter'; }
      if(statusLbl) { statusLbl.textContent = 'UV_ON'; statusLbl.className = 'font-label-micro text-[8px] text-status-standby font-mono font-bold'; }
      document.documentElement.classList.add('light-pcb');
    } else {
      // Actuate switch to LEFT (DARK / Silicon Core)
      switchLever.style.transform = 'translateX(0px)';
      ledIndicator.className = 'w-2.5 h-2.5 rounded-full bg-status-active shadow-[0_0_8px_#00FF66] transition-all duration-300 border border-status-active/50';
      if(posDark) { posDark.className = 'font-label-micro text-[8px] text-status-active font-mono font-bold tracking-tighter'; }
      if(posLight) { posLight.className = 'font-label-micro text-[8px] text-silkscreen-subtle font-mono'; }
      if(statusLbl) { statusLbl.textContent = 'PWR'; statusLbl.className = 'font-label-micro text-[8px] text-silkscreen-bright font-mono font-bold'; }
      document.documentElement.classList.remove('light-pcb');
    }
  });
}
</script>
</body></html>