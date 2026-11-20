<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <meta name="artifact-type" content="tool">
  <meta name="design-style" content="sticker">
  <title>지식의 탑 마스터 — 고1 통합사회2 기말고사 1등급 대비</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&family=Noto+Sans+KR:wght@400;500;700;900&display=swap" rel="stylesheet">
  <script src="https://unpkg.com/lucide@1.43.0/dist/umd/lucide.min.js"></script>
  <style>
    :root {
      color-scheme: light;

      /* 1. Sticker style tokens */
      --background: #fef7ff;
      --surface-container-low: #ffffff;
      --surface-container: #f8eef8;
      --surface-container-high: #f2e8f2;

      --on-surface: #2e1a28;
      --on-surface-variant: #604868;

      --outline: #907898;
      --outline-variant: #dcc8e0;

      --primary: #c2207f;
      --on-primary: #ffffff;
      --primary-container: #f080c0;
      --primary-container-soft: #fde4f3;
      --on-primary-container: #2e1a28;
      --secondary: #7c52aa;
      --on-secondary: #ffffff;
      --secondary-container: #efe5fa;
      --tertiary: #0096cc;
      --tertiary-container: #dff4fc;
      --tangerine: #d96a00;
      --tangerine-container: #ffedd5;
      --tangerine-ink: #9a3412;

      --error: #c53030;
      --error-container: #fee2e2;
      --on-error: #ffffff;

      --data-1: #c2207f;
      --data-2: #7c52aa;
      --data-3: #0096cc;
      --data-4: #d96a00;
      --data-context: #c8b8d0;

      /* 2. Fonts (Korean first + DM Sans) */
      --font-headline: 'Noto Sans KR', 'DM Sans', sans-serif;
      --font-body: 'Noto Sans KR', 'DM Sans', sans-serif;
      --font-label: 'Noto Sans KR', 'DM Sans', sans-serif;

      /* Shape */
      --rounded: 1rem;
      --rounded-lg: 2rem;
      --rounded-full: 9999px;

      /* Style effects */
      --shadow-pink: 0 4px 16px rgb(224 64 160 / 0.2);
      --shadow-pink-deep: 0 10px 28px rgb(224 64 160 / 0.32);
      --shadow-grape: 0 4px 16px rgb(124 82 170 / 0.2);
      --shadow-grape-deep: 0 10px 28px rgb(124 82 170 / 0.3);
      --shadow-sky: 0 4px 16px rgb(0 150 204 / 0.2);
      --shadow-positive: 0 4px 16px rgb(21 128 61 / 0.2);
      --shadow-error: 0 4px 16px rgb(197 48 48 / 0.22);
      --pop-scale: scale(1.03);
      --press-scale: scale(0.97);
      --lift: translateY(-4px);
      --ease-bounce: cubic-bezier(0.34, 1.56, 0.64, 1);

      /* 3. Shared Foundation Tokens */
      --positive: #15803d;
      --positive-container: #dcfce7;
      --warning: #b45309;
      --warning-container: #fef3c7;
      --focus: var(--primary);

      /* Type scale (Focused Tool) */
      --display-size: clamp(1.85rem, 1.4rem + 1.8vw, 2.65rem);
      --headline-size: clamp(1.25rem, 1.1rem + 0.55vw, 1.55rem);
      --subhead-size: clamp(1.0625rem, 1rem + 0.25vw, 1.2rem);
      --body-size: clamp(0.9375rem, 0.9rem + 0.15vw, 1rem);
      --label-size: 0.78rem;

      /* Spacing scale (4pt base) */
      --space-xs: 0.25rem;
      --space-sm: 0.5rem;
      --space-md: 1rem;
      --space-lg: 1.5rem;
      --space-xl: 2.5rem;
      --space-2xl: 4rem;
      --space-3xl: 6rem;

      /* Motion */
      --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
      --ease-in-out: cubic-bezier(0.65, 0, 0.35, 1);
      --dur-micro: 120ms;
      --dur-short: 220ms;
      --dur-long: 420ms;
    }

    /* Base reset */
    *, *::before, *::after { box-sizing: border-box; }
    html, body {
      overflow-x: clip;
      margin: 0;
      padding: 0;
      background-color: var(--background);
      color: var(--on-surface);
      font-family: var(--font-body);
      font-size: var(--body-size);
      line-height: 1.65;
      word-break: keep-all;
      overflow-wrap: break-word;
      -webkit-tap-highlight-color: transparent;
    }
    header { position: static !important; }

    button, input, select, textarea {
      font-family: inherit;
      font-size: inherit;
      color: inherit;
    }

    :focus-visible {
      outline: 3px solid var(--focus);
      outline-offset: 2px;
    }

    /* Page Grid Container */
    .page-grid {
      display: grid;
      grid-template-columns: minmax(0, 1fr);
      gap: var(--space-lg);
      padding: var(--space-lg);
      padding-left: max(var(--space-lg), env(safe-area-inset-left));
      padding-right: max(var(--space-lg), env(safe-area-inset-right));
      padding-bottom: max(var(--space-2xl), env(safe-area-inset-bottom));
      max-width: 1200px;
      margin: 0 auto;
      overflow: hidden;
    }
    .page-grid * { min-width: 0; }

    /* Hero Header */
    .app-header {
      max-width: 1200px;
      margin: 0 auto;
      padding: var(--space-xl) var(--space-lg) var(--space-sm);
      padding-left: max(var(--space-lg), env(safe-area-inset-left));
      padding-right: max(var(--space-lg), env(safe-area-inset-right));
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      gap: var(--space-sm);
    }

    .eyebrow-row {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: var(--space-sm);
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: var(--space-xs);
      background: var(--primary-container);
      color: var(--on-primary-container);
      border-radius: var(--rounded-full);
      padding: var(--space-xs) var(--space-md);
      font-size: var(--label-size);
      font-weight: 700;
      letter-spacing: 0;
      text-transform: none;
    }

    .badge.grape {
      background: var(--secondary-container);
      color: var(--secondary);
    }

    .badge.sky {
      background: var(--tertiary-container);
      color: var(--on-surface);
    }

    .badge.tangerine {
      background: var(--tangerine-container);
      color: var(--tangerine-ink);
    }

    .badge.positive {
      background: var(--positive-container);
      color: var(--positive);
    }

    .display {
      font-family: var(--font-headline);
      font-weight: 900;
      font-size: var(--display-size);
      line-height: 1.15;
      margin: 0;
      color: var(--on-surface);
    }

    .display em {
      font-style: normal;
      color: var(--primary);
    }

    .hero-lede {
      margin: 0;
      color: var(--on-surface-variant);
      max-width: 65ch;
      font-size: var(--body-size);
    }

    /* HUD Metrics Grid */
    .hud-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(min(210px, 100%), 1fr));
      gap: var(--space-md);
    }

    .card {
      background: var(--surface-container-low);
      border-radius: var(--rounded);
      box-shadow: var(--shadow-pink);
      padding: var(--space-lg);
      transition: transform var(--dur-short) var(--ease-bounce), box-shadow var(--dur-short) var(--ease-out);
    }
    .card.shadow-sky { box-shadow: var(--shadow-sky); }
    .card.shadow-grape { box-shadow: var(--shadow-grape); }

    .hud-card {
      padding: var(--space-md) var(--space-lg);
      display: flex;
      flex-direction: column;
      gap: var(--space-xs);
    }
    .hud-card:nth-child(3n+2) { box-shadow: var(--shadow-sky); }
    .hud-card:nth-child(3n+3) { box-shadow: var(--shadow-grape); }

    .hud-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
    }

    .hud-label {
      font-family: var(--font-label);
      font-size: var(--label-size);
      font-weight: 700;
      color: var(--on-surface-variant);
    }

    .hud-icon {
      width: 2rem;
      height: 2rem;
      border-radius: var(--rounded-full);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      background: var(--primary-container-soft);
      color: var(--primary);
      flex-shrink: 0;
    }
    .hud-card:nth-child(3n+2) .hud-icon {
      background: var(--tertiary-container);
      color: var(--on-surface);
    }
    .hud-card:nth-child(3n+3) .hud-icon {
      background: var(--secondary-container);
      color: var(--secondary);
    }

    .hud-value {
      font-size: clamp(1.4rem, 1.2rem + 0.8vw, 1.85rem);
      font-weight: 900;
      font-variant-numeric: tabular-nums;
      line-height: 1.15;
      color: var(--on-surface);
    }
    .hud-value.accent { color: var(--primary); }

    .hud-sub {
      font-size: var(--label-size);
      color: var(--on-surface-variant);
    }

    /* Lollipop Progress Track */
    .progress-track {
      width: 100%;
      height: 0.625rem;
      background: var(--surface-container-high);
      border-radius: var(--rounded-full);
      overflow: hidden;
      margin-top: var(--space-xs);
    }

    .progress-fill {
      height: 100%;
      width: 0%;
      background: var(--primary);
      border-radius: var(--rounded-full);
      transition: width var(--dur-long) var(--ease-bounce);
    }
    .progress-fill.sky { background: var(--tertiary); }
    .progress-fill.grape { background: var(--secondary); }

    /* Mode Segmented Switcher */
    .mode-nav-wrap {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-md);
    }

    .segmented {
      display: inline-flex;
      flex-wrap: wrap;
      gap: var(--space-xs);
      background: var(--surface-container-high);
      padding: var(--space-xs);
      border-radius: var(--rounded-full);
      max-width: 100%;
    }

    .seg-btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: var(--space-sm);
      min-height: 44px;
      padding: var(--space-sm) var(--space-lg);
      border: 0;
      border-radius: var(--rounded-full);
      background: transparent;
      color: var(--on-surface-variant);
      font-weight: 700;
      font-size: var(--body-size);
      cursor: pointer;
      transition: transform var(--dur-short) var(--ease-bounce),
                  background-color var(--dur-short) var(--ease-out),
                  color var(--dur-short) var(--ease-out),
                  box-shadow var(--dur-short) var(--ease-out);
    }
    .seg-btn:hover {
      color: var(--on-surface);
      transform: var(--pop-scale);
    }
    .seg-btn:active { transform: var(--press-scale); }
    .seg-btn.active {
      background: var(--primary);
      color: var(--on-primary);
      box-shadow: var(--shadow-pink);
    }

    /* Buttons & Chips */
    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: var(--space-sm);
      min-height: 44px;
      padding: var(--space-sm) var(--space-lg);
      border: 0;
      border-radius: var(--rounded-full);
      font-weight: 700;
      cursor: pointer;
      transition: transform var(--dur-short) var(--ease-bounce),
                  box-shadow var(--dur-short) var(--ease-out),
                  background-color var(--dur-short) var(--ease-out);
    }
    .btn:hover:not(:disabled) { transform: var(--pop-scale); }
    .btn:active:not(:disabled) { transform: var(--press-scale); }
    .btn:disabled {
      opacity: 0.48;
      cursor: not-allowed;
      transform: none;
    }

    .btn-primary {
      background: var(--primary);
      color: var(--on-primary);
      box-shadow: var(--shadow-pink);
    }
    .btn-primary:hover:not(:disabled) { box-shadow: var(--shadow-pink-deep); }

    .btn-secondary {
      background: var(--secondary);
      color: var(--on-secondary);
      box-shadow: var(--shadow-grape);
    }
    .btn-secondary:hover:not(:disabled) { box-shadow: var(--shadow-grape-deep); }

    .btn-soft {
      background: var(--surface-container);
      color: var(--on-surface);
    }
    .btn-soft:hover:not(:disabled) { background: var(--surface-container-high); }

    .btn-quiet {
      background: transparent;
      color: var(--primary);
      padding: var(--space-sm) var(--space-md);
    }
    .btn-quiet:hover:not(:disabled) { background: var(--primary-container-soft); }

    .btn-danger-soft {
      background: var(--error-container);
      color: var(--error);
    }

    .chip-row {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: var(--space-sm);
    }

    .chip {
      display: inline-flex;
      align-items: center;
      gap: var(--space-xs);
      min-height: 44px;
      padding: var(--space-xs) var(--space-md);
      border-radius: var(--rounded-full);
      border: 2px solid var(--outline-variant);
      background: var(--surface-container-low);
      color: var(--on-surface-variant);
      font-weight: 700;
      font-size: var(--label-size);
      cursor: pointer;
      transition: transform var(--dur-short) var(--ease-bounce),
                  background-color var(--dur-short) var(--ease-out),
                  color var(--dur-short) var(--ease-out),
                  box-shadow var(--dur-short) var(--ease-out);
    }
    .chip:hover {
      transform: var(--pop-scale);
      color: var(--on-surface);
    }
    .chip:active { transform: var(--press-scale); }
    .chip.active {
      background: var(--secondary);
      border-color: var(--secondary);
      color: var(--on-secondary);
      box-shadow: var(--shadow-grape);
    }
    .chip.wrong-filter.active {
      background: var(--error);
      border-color: var(--error);
      color: var(--on-error);
      box-shadow: var(--shadow-error);
    }

    /* Mode Panels */
    .mode-panel { display: none; }
    .mode-panel.active {
      display: grid;
      grid-template-columns: minmax(0, 1fr);
      gap: var(--space-lg);
      animation: panelEnter var(--dur-long) var(--ease-out) both;
    }

    @keyframes panelEnter {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* ========================================
       MODE 1: TOWER QUIZ ARENA
       ======================================== */
    .tower-arena {
      display: grid;
      grid-template-columns: minmax(0, 0.92fr) minmax(0, 1.28fr);
      gap: var(--space-lg);
      align-items: start;
    }

    @media (max-width: 900px) {
      .tower-arena {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .tower-stage-card {
      background: var(--surface-container-low);
      border-radius: var(--rounded-lg);
      box-shadow: var(--shadow-grape);
      padding: var(--space-lg);
      display: flex;
      flex-direction: column;
      gap: var(--space-md);
    }

    .stage-header {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
    }

    .section-title {
      font-family: var(--font-headline);
      font-weight: 800;
      font-size: var(--headline-size);
      margin: 0;
      color: var(--on-surface);
      line-height: 1.25;
    }

    .tier-banner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
      background: var(--surface-container);
      border-radius: var(--rounded);
      padding: var(--space-sm) var(--space-md);
      font-size: var(--label-size);
      font-weight: 700;
      color: var(--on-surface);
    }

    .tower-viewport {
      background: var(--surface-container);
      border-radius: var(--rounded);
      padding: var(--space-md);
      min-height: 360px;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      gap: var(--space-xs);
      position: relative;
      overflow: hidden;
    }

    .tower-sky-goal {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: var(--space-xs) var(--space-sm);
      border-radius: var(--rounded-full);
      background: var(--surface-container-low);
      color: var(--primary);
      font-size: var(--label-size);
      font-weight: 800;
      margin-bottom: auto;
      box-shadow: var(--shadow-pink);
    }

    .tower-stack {
      display: flex;
      flex-direction: column-reverse;
      gap: var(--space-xs);
      width: 100%;
      align-items: center;
    }

    .tower-block {
      width: 100%;
      max-width: 96%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
      padding: var(--space-xs) var(--space-md);
      border-radius: var(--rounded-full);
      font-size: var(--label-size);
      font-weight: 700;
      color: var(--on-surface);
      background: var(--primary-container);
      box-shadow: var(--shadow-pink);
      animation: blockStack var(--dur-long) var(--ease-bounce) both;
    }
    .tower-block.unit-market {
      background: var(--primary-container);
      color: var(--on-primary-container);
      box-shadow: var(--shadow-pink);
    }
    .tower-block.unit-global {
      background: var(--tertiary-container);
      color: var(--on-surface);
      box-shadow: var(--shadow-sky);
    }
    .tower-block.unit-climate {
      background: var(--secondary-container);
      color: var(--secondary);
      box-shadow: var(--shadow-grape);
    }
    .tower-block.unit-justice {
      background: var(--tangerine-container);
      color: var(--tangerine-ink);
      box-shadow: var(--shadow-pink);
    }

    .tower-block.crumbling {
      animation: blockShake var(--dur-long) var(--ease-out) both;
      background: var(--error-container);
      color: var(--error);
    }

    @keyframes blockStack {
      from { opacity: 0; transform: translateY(-18px) scale(0.92); }
      to { opacity: 1; transform: translateY(0) scale(1); }
    }

    @keyframes blockShake {
      0%, 100% { transform: translateX(0); }
      25% { transform: translateX(-8px); }
      50% { transform: translateX(8px); }
      75% { transform: translateX(-5px); }
    }

    .tower-empty-hint {
      text-align: center;
      padding: var(--space-lg) var(--space-md);
      color: var(--on-surface-variant);
      font-size: var(--label-size);
      font-weight: 500;
      border: 2px dashed var(--outline-variant);
      border-radius: var(--rounded);
      width: 100%;
    }

    .tower-foundation {
      width: 100%;
      padding: var(--space-sm) var(--space-md);
      border-radius: var(--rounded-full);
      background: var(--on-surface);
      color: var(--on-primary);
      text-align: center;
      font-size: var(--label-size);
      font-weight: 800;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: var(--space-xs);
    }

    .tower-event-banner {
      padding: var(--space-sm) var(--space-md);
      border-radius: var(--rounded);
      font-size: var(--label-size);
      font-weight: 700;
      display: flex;
      align-items: center;
      gap: var(--space-sm);
      background: var(--surface-container);
      color: var(--on-surface-variant);
    }
    .tower-event-banner.gain {
      background: var(--positive-container);
      color: var(--positive);
    }
    .tower-event-banner.loss {
      background: var(--error-container);
      color: var(--error);
    }

    /* Quiz Card */
    .quiz-card {
      background: var(--surface-container-low);
      border-radius: var(--rounded-lg);
      box-shadow: var(--shadow-pink);
      padding: var(--space-xl);
      display: flex;
      flex-direction: column;
      gap: var(--space-lg);
    }

    .quiz-meta {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
    }

    .quiz-question {
      font-family: var(--font-headline);
      font-weight: 800;
      font-size: clamp(1.125rem, 1rem + 0.45vw, 1.35rem);
      line-height: 1.5;
      margin: 0;
      color: var(--on-surface);
    }

    .quiz-context-box {
      background: var(--surface-container);
      border-radius: var(--rounded);
      padding: var(--space-md) var(--space-lg);
      font-size: var(--body-size);
      color: var(--on-surface);
    }

    .options-list {
      display: grid;
      grid-template-columns: minmax(0, 1fr);
      gap: var(--space-sm);
    }

    .option-btn {
      width: 100%;
      min-height: 52px;
      text-align: left;
      display: flex;
      align-items: center;
      gap: var(--space-md);
      padding: var(--space-md) var(--space-lg);
      border-radius: var(--rounded);
      border: 2px solid var(--outline-variant);
      background: var(--surface-container-low);
      color: var(--on-surface);
      font-weight: 500;
      cursor: pointer;
      transition: transform var(--dur-short) var(--ease-bounce),
                  background-color var(--dur-short) var(--ease-out),
                  box-shadow var(--dur-short) var(--ease-out);
    }
    .option-btn:hover:not(:disabled) {
      transform: translateY(-2px);
      background: var(--surface-container);
      box-shadow: var(--shadow-pink);
    }
    .option-btn:active:not(:disabled) { transform: var(--press-scale); }
    .option-btn:disabled { cursor: default; }

    .option-num {
      width: 2rem;
      height: 2rem;
      border-radius: var(--rounded-full);
      background: var(--surface-container-high);
      color: var(--on-surface);
      font-weight: 800;
      font-size: var(--label-size);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
    }

    .option-btn.correct {
      background: var(--positive-container);
      border-color: var(--positive);
      color: var(--on-surface);
      box-shadow: var(--shadow-positive);
    }
    .option-btn.correct .option-num {
      background: var(--positive);
      color: var(--on-primary);
    }

    .option-btn.wrong {
      background: var(--error-container);
      border-color: var(--error);
      color: var(--on-surface);
      box-shadow: var(--shadow-error);
    }
    .option-btn.wrong .option-num {
      background: var(--error);
      color: var(--on-error);
    }

    .explanation-box {
      background: var(--surface-container);
      border-radius: var(--rounded);
      padding: var(--space-lg);
      display: flex;
      flex-direction: column;
      gap: var(--space-sm);
    }
    .explanation-box.is-correct {
      background: var(--positive-container);
    }
    .explanation-box.is-wrong {
      background: var(--error-container);
    }

    .explanation-title {
      display: flex;
      align-items: center;
      gap: var(--space-sm);
      font-weight: 800;
      font-size: var(--subhead-size);
    }

    .quiz-footer {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-md);
    }

    /* ========================================
       MODE 2: FLASHCARD TRAINER
       ======================================== */
    .flash-workspace {
      display: grid;
      grid-template-columns: minmax(0, 1fr);
      gap: var(--space-lg);
    }

    .flash-toolbar {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-md);
    }

    .flash-stage {
      perspective: 1200px;
      width: 100%;
      max-width: 760px;
      margin: 0 auto;
    }

    .flashcard {
      position: relative;
      width: 100%;
      min-height: 300px;
      cursor: pointer;
      transform-style: preserve-3d;
      transition: transform var(--dur-long) var(--ease-bounce);
      border-radius: var(--rounded-lg);
      border: 0;
      background: transparent;
      padding: 0;
      text-align: left;
      display: block;
    }
    .flashcard.flipped {
      transform: rotateY(180deg);
    }

    .flash-face {
      position: absolute;
      inset: 0;
      backface-visibility: hidden;
      -webkit-backface-visibility: hidden;
      background: var(--surface-container-low);
      border-radius: var(--rounded-lg);
      box-shadow: var(--shadow-pink);
      padding: var(--space-xl);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      gap: var(--space-md);
    }

    .flash-face.back {
      transform: rotateY(180deg);
      box-shadow: var(--shadow-grape);
      background: var(--surface-container-low);
    }

    .flash-term {
      font-family: var(--font-headline);
      font-weight: 900;
      font-size: clamp(1.45rem, 1.2rem + 1vw, 2rem);
      color: var(--on-surface);
      margin: 0;
      line-height: 1.25;
    }

    .flash-prompt {
      color: var(--on-surface-variant);
      margin: 0;
      font-size: var(--body-size);
    }

    .flash-answer {
      font-size: clamp(1rem, 0.95rem + 0.25vw, 1.125rem);
      color: var(--on-surface);
      margin: 0;
      line-height: 1.65;
    }

    .flash-controls {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
      gap: var(--space-sm);
    }

    .term-dots {
      display: flex;
      flex-wrap: wrap;
      gap: var(--space-xs);
      justify-content: center;
    }

    .term-pill {
      min-height: 36px;
      padding: var(--space-xs) var(--space-md);
      border-radius: var(--rounded-full);
      border: 0;
      background: var(--surface-container);
      color: var(--on-surface-variant);
      font-size: var(--label-size);
      font-weight: 700;
      cursor: pointer;
      transition: transform var(--dur-short) var(--ease-bounce), background-color var(--dur-short) var(--ease-out);
    }
    .term-pill:hover { transform: var(--pop-scale); }
    .term-pill.current {
      background: var(--primary);
      color: var(--on-primary);
    }
    .term-pill.mastered {
      background: var(--positive-container);
      color: var(--positive);
    }
    .term-pill.current.mastered {
      background: var(--primary);
      color: var(--on-primary);
    }

    /* ========================================
       MODE 3: SUMMARY NOTES & CALCULATOR
       ======================================== */
    .summary-toolbar {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-md);
      background: var(--surface-container-low);
      border-radius: var(--rounded);
      box-shadow: var(--shadow-sky);
      padding: var(--space-md) var(--space-lg);
    }

    .switch-btn {
      display: inline-flex;
      align-items: center;
      gap: var(--space-sm);
      min-height: 44px;
      padding: var(--space-xs) var(--space-md);
      border-radius: var(--rounded-full);
      border: 0;
      background: var(--surface-container-high);
      color: var(--on-surface);
      font-weight: 700;
      cursor: pointer;
      transition: background-color var(--dur-short) var(--ease-out), transform var(--dur-short) var(--ease-bounce);
    }
    .switch-btn:hover { transform: var(--pop-scale); }
    .switch-btn[aria-pressed="true"] {
      background: var(--primary);
      color: var(--on-primary);
      box-shadow: var(--shadow-pink);
    }

    .summary-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(min(340px, 100%), 1fr));
      gap: var(--space-lg);
    }

    .summary-card {
      background: var(--surface-container-low);
      border-radius: var(--rounded-lg);
      box-shadow: var(--shadow-pink);
      padding: var(--space-xl);
      display: flex;
      flex-direction: column;
      gap: var(--space-md);
    }
    .summary-card:nth-child(3n+2) { box-shadow: var(--shadow-sky); }
    .summary-card:nth-child(3n+3) { box-shadow: var(--shadow-grape); }

    .summary-list {
      margin: 0;
      padding-left: var(--space-lg);
      display: flex;
      flex-direction: column;
      gap: var(--space-sm);
    }

    /* Blank / Active Recall Chips */
    .blank-chip {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 0 var(--space-sm);
      margin: 0 var(--space-xs);
      min-height: 28px;
      border-radius: var(--rounded-full);
      border: 0;
      background: var(--primary-container-soft);
      color: var(--primary);
      font-weight: 800;
      cursor: pointer;
      transition: transform var(--dur-short) var(--ease-bounce), background-color var(--dur-short) var(--ease-out);
      vertical-align: baseline;
    }
    .blank-chip:hover { transform: var(--pop-scale); }
    .blank-chip.hidden-answer {
      background: var(--primary);
      color: var(--on-primary);
      min-width: 72px;
    }

    /* Clean Table */
    .table-wrap {
      width: 100%;
      overflow-x: auto;
    }
    .clean-table {
      width: 100%;
      border-collapse: collapse;
      font-size: var(--label-size);
    }
    .clean-table th {
      background: var(--surface-container);
      color: var(--on-surface-variant);
      font-weight: 800;
      text-align: left;
      padding: var(--space-sm) var(--space-md);
    }
    .clean-table th:first-child { border-radius: var(--rounded) 0 0 var(--rounded); }
    .clean-table th:last-child { border-radius: 0 var(--rounded) var(--rounded) 0; }
    .clean-table td {
      padding: var(--space-sm) var(--space-md);
      vertical-align: top;
      color: var(--on-surface);
    }
    .clean-table tbody tr:nth-child(even) td {
      background: var(--surface-container);
    }

    /* Mini Opportunity Cost Simulator */
    .calc-panel {
      background: var(--surface-container);
      border-radius: var(--rounded);
      padding: var(--space-lg);
      display: flex;
      flex-direction: column;
      gap: var(--space-md);
    }

    .calc-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(min(180px, 100%), 1fr));
      gap: var(--space-md);
      align-items: end;
    }

    .field-group {
      display: flex;
      flex-direction: column;
      gap: var(--space-xs);
    }

    .field-label {
      font-size: var(--label-size);
      font-weight: 700;
      color: var(--on-surface-variant);
    }

    .pill-input {
      width: 100%;
      min-height: 44px;
      padding: var(--space-sm) var(--space-md);
      border-radius: var(--rounded-full);
      border: 2px solid var(--outline);
      background: var(--surface-container-low);
      color: var(--on-surface);
      font-weight: 700;
      font-variant-numeric: tabular-nums;
    }
    .pill-input:focus {
      border-color: var(--primary);
      outline: 3px solid var(--focus);
      outline-offset: 2px;
    }

    .calc-result {
      background: var(--surface-container-low);
      border-radius: var(--rounded);
      padding: var(--space-md);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
    }

    .trap-callout {
      background: var(--warning-container);
      color: var(--on-surface);
      border-radius: var(--rounded);
      padding: var(--space-md);
      font-size: var(--label-size);
      display: flex;
      align-items: flex-start;
      gap: var(--space-sm);
    }
    .trap-callout strong { color: var(--warning); }

    /* Celebration Banner */
    .victory-banner {
      background: var(--primary-container-soft);
      border-radius: var(--rounded);
      padding: var(--space-md) var(--space-lg);
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-sm);
      color: var(--on-surface);
      font-weight: 700;
    }

    /* Footer Source Note */
    .source-note {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 var(--space-lg) var(--space-2xl);
      color: var(--on-surface-variant);
      font-size: var(--label-size);
    }

    /* Container Queries */
    .card-wrapper { container-type: inline-size; }
    @container (max-width: 440px) {
      .quiz-card, .summary-card, .flash-face {
        padding: var(--space-lg);
      }
    }

    /* Mobile Breakpoint */
    @media (max-width: 640px) {
      .page-grid {
        padding: var(--space-md);
        gap: var(--space-md);
      }
      .app-header {
        padding: var(--space-lg) var(--space-md) var(--space-xs);
      }
      .quiz-card, .summary-card, .tower-stage-card {
        padding: var(--space-md);
      }
      .segmented {
        width: 100%;
      }
      .seg-btn {
        flex: 1 1 auto;
        padding: var(--space-xs) var(--space-sm);
        font-size: var(--label-size);
      }
      .tower-viewport {
        min-height: 240px;
      }
      .flashcard {
        min-height: 340px;
      }
    }

    /* Reduced Motion */
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
      }
    }
  </style>
</head>
<body>

  <header class="app-header">
    <div class="eyebrow-row">
      <span class="badge"><i data-lucide="award" aria-hidden="true" width="15" height="15"></i> 고1 통합사회2 기말고사 1등급 대비</span>
      <span class="badge sky"><i data-lucide="smartphone" aria-hidden="true" width="15" height="15"></i> PC · 태블릿 · 모바일 자동 최적화</span>
    </div>
    <h1 class="display">지식의 <em>탑</em> 마스터</h1>
    <p class="hero-lede">문제를 맞히면 지식의 탑이 한 층씩 쌓이고, 틀리면 블록이 깎이는 실전 타워 퀴즈와 플래시카드·핵심 요약 노트로 통합사회2 기말고사 전 범위를 정복하세요.</p>
  </header>

  <main class="page-grid">

    <!-- 상단 HUD 현황판 -->
    <section aria-label="학습 현황 요약" class="hud-grid">
      <div class="card hud-card">
        <div class="hud-top">
          <span class="hud-label">현재 지식의 탑</span>
          <span class="hud-icon"><i data-lucide="building-2" aria-hidden="true" width="16" height="16"></i></span>
        </div>
        <div class="hud-value accent" id="hud-floor">0F</div>
        <div class="hud-sub" id="hud-floor-sub">목표 15F (1등급 마스터)</div>
        <div class="progress-track" aria-hidden="true">
          <div class="progress-fill" id="hud-floor-bar"></div>
        </div>
      </div>

      <div class="card hud-card">
        <div class="hud-top">
          <span class="hud-label">누적 획득 점수</span>
          <span class="hud-icon"><i data-lucide="sparkles" aria-hidden="true" width="16" height="16"></i></span>
        </div>
        <div class="hud-value" id="hud-score">0점</div>
        <div class="hud-sub" id="hud-streak">연속 정답 0콤보 · 최고 0콤보</div>
      </div>

      <div class="card hud-card">
        <div class="hud-top">
          <span class="hud-label">핵심 용어 암기</span>
          <span class="hud-icon"><i data-lucide="layers" aria-hidden="true" width="16" height="16"></i></span>
        </div>
        <div class="hud-value" id="hud-cards">0 / 18</div>
        <div class="hud-sub" id="hud-cards-sub">플래시카드 완성도 0%</div>
        <div class="progress-track" aria-hidden="true">
          <div class="progress-fill grape" id="hud-cards-bar"></div>
        </div>
      </div>

      <div class="card hud-card">
        <div class="hud-top">
          <span class="hud-label">최고 탑 기록 · 오답</span>
          <span class="hud-icon"><i data-lucide="trophy" aria-hidden="true" width="16" height="16"></i></span>
        </div>
        <div class="hud-value" id="hud-best">최고 0F</div>
        <div class="hud-sub" id="hud-wrong">오답 노트 0문항</div>
      </div>
    </section>

    <!-- 학습 모드 전환 세그먼트 바 -->
    <nav aria-label="학습 모드 선택" class="mode-nav-wrap">
      <div class="segmented" role="tablist">
        <button type="button" class="seg-btn active" id="tab-tower" role="tab" aria-selected="true" onclick="switchMode('tower')">
          <i data-lucide="castle" aria-hidden="true" width="18" height="18"></i>
          지식의 탑 퀴즈
        </button>
        <button type="button" class="seg-btn" id="tab-flashcard" role="tab" aria-selected="false" onclick="switchMode('flashcard')">
          <i data-lucide="copy" aria-hidden="true" width="18" height="18"></i>
          용어 플래시카드
        </button>
        <button type="button" class="seg-btn" id="tab-summary" role="tab" aria-selected="false" onclick="switchMode('summary')">
          <i data-lucide="book-open" aria-hidden="true" width="18" height="18"></i>
          핵심 내용 요약
        </button>
      </div>
    </nav>

    <!-- =====================================
         MODE 1: 지식의 탑 게임형 문제 풀이
         ===================================== -->
    <section id="panel-tower" class="mode-panel active" aria-labelledby="tab-tower">
      <div class="chip-row" role="group" aria-label="문제 단원 필터">
        <button type="button" class="chip active" data-quiz-filter="all" onclick="setQuizFilter('all')">전체 범위 (16문항)</button>
        <button type="button" class="chip" data-quiz-filter="market" onclick="setQuizFilter('market')">시장경제·합리적 선택</button>
        <button type="button" class="chip" data-quiz-filter="global" onclick="setQuizFilter('global')">세계화·국제무역</button>
        <button type="button" class="chip" data-quiz-filter="climate" onclick="setQuizFilter('climate')">기후변화·지속가능성</button>
        <button type="button" class="chip" data-quiz-filter="justice" onclick="setQuizFilter('justice')">정의와 인권</button>
        <button type="button" class="chip wrong-filter" data-quiz-filter="wrong" id="btn-wrong-filter" onclick="setQuizFilter('wrong')">오답 집중 복습 (0)</button>
      </div>

      <div id="victory-banner" class="victory-banner" style="display: none;">
        <span><i data-lucide="crown" aria-hidden="true" width="18" height="18"></i> 축하합니다! 15층 '1등급 마스터 지식의 탑'을 완공했습니다! 계속 문제를 풀며 최고 층수를 경신해 보세요.</span>
        <span class="badge positive">1등급 달성</span>
      </div>

      <div class="tower-arena card-wrapper">
        <!-- 좌측: 인터랙티브 지식의 탑 시각화 -->
        <div class="tower-stage-card">
          <div class="stage-header">
            <h2 class="section-title">나의 지식의 탑</h2>
            <button type="button" class="btn btn-soft" id="btn-reset-tower" onclick="handleResetTower(this)">
              <i data-lucide="rotate-ccw" aria-hidden="true" width="16" height="16"></i>
              탑 초기화
            </button>
          </div>

          <div class="tier-banner">
            <span id="tower-rank-label">현재 등급: 기초 공사 중 (0F)</span>
            <span id="tower-next-goal">다음 목표: 5F 브론즈 탑</span>
          </div>

          <div id="tower-event-banner" class="tower-event-banner">
            <i data-lucide="info" aria-hidden="true" width="16" height="16"></i>
            <span>정답 시 +1층 &amp; +100점(콤보 보너스), 오답 시 -1층 &amp; -50점 감점됩니다.</span>
          </div>

          <div class="tower-viewport" aria-live="polite">
            <div class="tower-sky-goal">
              <span><i data-lucide="flag" aria-hidden="true" width="14" height="14"></i> 목표: 15F 1등급 완공</span>
              <span id="tower-height-badge">0 / 15층</span>
            </div>

            <div class="tower-stack" id="tower-stack"></div>

            <div class="tower-foundation">
              <i data-lucide="shield-check" aria-hidden="true" width="16" height="16"></i>
              통합사회2 1등급 기초 토대
            </div>
          </div>
        </div>

        <!-- 우측: 실전 퀴즈 스테이지 -->
        <div class="quiz-card" id="quiz-stage">
          <div class="quiz-meta">
            <div class="eyebrow-row">
              <span class="badge grape" id="quiz-unit-badge">시장경제</span>
              <span class="badge tangerine" id="quiz-diff-badge">1등급 변별력</span>
            </div>
            <span class="hud-label" id="quiz-counter">문제 1 / 16</span>
          </div>

          <h3 class="quiz-question" id="quiz-question">문제를 불러오는 중…</h3>

          <div class="quiz-context-box" id="quiz-context" style="display: none;"></div>

          <div class="options-list" id="quiz-options"></div>

          <div class="explanation-box" id="quiz-explanation" style="display: none;" aria-live="polite">
            <div class="explanation-title" id="exp-title"></div>
            <div id="exp-body"></div>
          </div>

          <div class="quiz-footer">
            <button type="button" class="btn btn-quiet" onclick="skipQuestion()">
              <i data-lucide="skip-forward" aria-hidden="true" width="16" height="16"></i>
              다른 문제 보기
            </button>
            <button type="button" class="btn btn-primary" id="btn-next-question" onclick="nextQuestion()" disabled>
              다음 문제 도전
              <i data-lucide="arrow-right" aria-hidden="true" width="16" height="16"></i>
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- =====================================
         MODE 2: 핵심 용어 플래시카드 학습
         ===================================== -->
    <section id="panel-flashcard" class="mode-panel" aria-labelledby="tab-flashcard">
      <div class="flash-toolbar">
        <div class="chip-row" role="group" aria-label="플래시카드 단원 필터">
          <button type="button" class="chip active" data-card-filter="all" onclick="setCardFilter('all')">전체 (18)</button>
          <button type="button" class="chip" data-card-filter="market" onclick="setCardFilter('market')">시장경제</button>
          <button type="button" class="chip" data-card-filter="global" onclick="setCardFilter('global')">세계화·무역</button>
          <button type="button" class="chip" data-card-filter="climate" onclick="setCardFilter('climate')">기후·지속가능</button>
          <button type="button" class="chip" data-card-filter="justice" onclick="setCardFilter('justice')">정의·인권</button>
          <button type="button" class="chip" data-card-filter="unmastered" onclick="setCardFilter('unmastered')">미암기만</button>
        </div>

        <div class="chip-row">
          <button type="button" class="btn btn-soft" onclick="shuffleCards()">
            <i data-lucide="shuffle" aria-hidden="true" width="16" height="16"></i>
            순서 섞기
          </button>
          <button type="button" class="btn btn-danger-soft" onclick="handleResetCards(this)">
            <i data-lucide="refresh-cw" aria-hidden="true" width="16" height="16"></i>
            암기 초기화
          </button>
        </div>
      </div>

      <div class="card shadow-sky" style="padding: var(--space-md) var(--space-lg);">
        <div class="hud-top">
          <span class="hud-label" id="flash-progress-label">현재 카드 1 / 18 · 전체 암기율 0%</span>
          <span class="badge positive" id="flash-mastered-badge" style="display: none;">암기 완료됨</span>
        </div>
        <div class="progress-track">
          <div class="progress-fill sky" id="flash-progress-bar"></div>
        </div>
      </div>

      <div class="flash-stage">
        <button type="button" class="flashcard" id="flashcard-btn" onclick="flipFlashcard()" aria-label="플래시카드 뒤집기">
          <span class="flash-face front">
            <span class="hud-top">
              <span class="badge grape" id="card-unit-front">시장경제</span>
              <span class="hud-label">앞면 · 탭하여 정답 확인</span>
            </span>
            <span>
              <h2 class="flash-term" id="card-term-front">매몰비용</h2>
              <p class="flash-prompt" id="card-question-front">질문 힌트</p>
            </span>
            <span class="hud-label"><i data-lucide="mouse-pointer-click" aria-hidden="true" width="14" height="14"></i> 클릭하거나 스페이스바를 눌러 뒤집기</span>
          </span>

          <span class="flash-face back">
            <span class="hud-top">
              <span class="badge" id="card-unit-back">핵심 정답 &amp; 출제 포인트</span>
              <span class="hud-label">뒷면 · 다시 탭하면 앞면</span>
            </span>
            <span>
              <h2 class="flash-term" id="card-term-back">매몰비용</h2>
              <p class="flash-answer" id="card-answer-back">정답 내용</p>
            </span>
            <span class="hud-label" id="card-tip-back">1등급 암기 팁</span>
          </span>
        </button>
      </div>

      <div class="flash-controls">
        <button type="button" class="btn btn-soft" onclick="prevFlashcard()">
          <i data-lucide="chevron-left" aria-hidden="true" width="18" height="18"></i>
          이전 카드
        </button>
        <button type="button" class="btn btn-secondary" onclick="markCardReview()">
          <i data-lucide="bookmark" aria-hidden="true" width="18" height="18"></i>
          다시 보기
        </button>
        <button type="button" class="btn btn-primary" onclick="markCardMastered()">
          <i data-lucide="check-circle-2" aria-hidden="true" width="18" height="18"></i>
          완벽 암기 (+20점)
        </button>
        <button type="button" class="btn btn-soft" onclick="nextFlashcard()">
          다음 카드
          <i data-lucide="chevron-right" aria-hidden="true" width="18" height="18"></i>
        </button>
      </div>

      <div class="term-dots" id="term-dots" aria-label="용어 목록 바로가기"></div>
    </section>

    <!-- =====================================
         MODE 3: 핵심 내용 요약 정리
         ===================================== -->
    <section id="panel-summary" class="mode-panel" aria-labelledby="tab-summary">
      <div class="summary-toolbar">
        <div>
          <h2 class="section-title" style="font-size: var(--subhead-size);">1등급 핵심 노트 &amp; 암기 가림막</h2>
          <span class="hud-label">가림막 모드를 켜고 분홍색 빈칸을 클릭하며 스스로 정답을 인출해 보세요.</span>
        </div>
        <div class="chip-row">
          <button type="button" class="switch-btn" id="btn-blank-toggle" aria-pressed="false" onclick="toggleBlankMode()">
            <i data-lucide="eye-off" aria-hidden="true" width="16" height="16"></i>
            <span id="blank-toggle-label">암기 가림막 OFF</span>
          </button>
          <button type="button" class="btn btn-soft" onclick="revealAllBlanks()">모두 열기</button>
        </div>
      </div>

      <div class="summary-grid">
        <!-- 카드 1: 합리적 선택 & 기회비용 계산기 -->
        <article class="summary-card">
          <div class="hud-top">
            <span class="badge">단원 1 · 시장경제</span>
            <span class="hud-label">필수 계산 공식</span>
          </div>
          <h3 class="section-title">합리적 선택과 비용 계산</h3>
          <ul class="summary-list">
            <li><strong>합리적 선택 조건</strong>: 최소 비용으로 최대 편익을 얻는 것으로, 반드시 <strong>편익 &gt; <button type="button" class="blank-chip" data-term="기회비용" onclick="toggleSingleBlank(this)">기회비용</button></strong>이어야 합니다.</li>
            <li><strong>기회비용 구성</strong>: 실제 지불한 <button type="button" class="blank-chip" data-term="명시적 비용" onclick="toggleSingleBlank(this)">명시적 비용</button> + 포기한 대안의 가치인 <button type="button" class="blank-chip" data-term="암묵적 비용" onclick="toggleSingleBlank(this)">암묵적 비용</button>.</li>
            <li><strong>매몰비용 원칙</strong>: 이미 지불해 회수 불가능한 <button type="button" class="blank-chip" data-term="매몰비용" onclick="toggleSingleBlank(this)">매몰비용</button>은 의사결정에서 <strong>전적으로 배제</strong>합니다.</li>
          </ul>

          <div class="calc-panel" aria-label="기회비용 미니 시뮬레이터">
            <span class="hud-label"><i data-lucide="calculator" aria-hidden="true" width="14" height="14"></i> 주은이의 선택! 기회비용 미니 시뮬레이터</span>
            <div class="calc-grid">
              <div class="field-group">
                <label class="field-label" for="calc-explicit">영화 티켓값 (원)</label>
                <input type="number" class="pill-input" id="calc-explicit" value="30000" min="0" step="1000" oninput="updateCostCalc()">
              </div>
              <div class="field-group">
                <label class="field-label" for="calc-wage">아르바이트 시급 (원)</label>
                <input type="number" class="pill-input" id="calc-wage" value="11000" min="0" step="500" oninput="updateCostCalc()">
              </div>
              <div class="field-group">
                <label class="field-label" for="calc-hours">빠지는 시간 (시간)</label>
                <input type="number" class="pill-input" id="calc-hours" value="2" min="0" max="12" step="1" oninput="updateCostCalc()">
              </div>
            </div>
            <div class="calc-result" id="calc-output">
              <span>총 기회비용: <strong style="color: var(--primary);">52,000원</strong></span>
              <span class="hud-label">편익이 52,000원 초과 시 합리적 선택</span>
            </div>
          </div>
        </article>

        <!-- 카드 2: 시장 실패와 정부/기업 -->
        <article class="summary-card">
          <div class="hud-top">
            <span class="badge sky">단원 2 · 시장 실패</span>
            <span class="hud-label">출제 1순위</span>
          </div>
          <h3 class="section-title">시장 실패 원인과 ESG 경영</h3>
          <ul class="summary-list">
            <li><strong>독과점</strong>: 소수 공급자가 가격·공급량을 임의 조절해 자원 배분이 비효율적이 됩니다.</li>
            <li><strong>공공재 부족</strong>: <button type="button" class="blank-chip" data-term="비배제성" onclick="toggleSingleBlank(this)">비배제성</button>과 <button type="button" class="blank-chip" data-term="비경쟁성" onclick="toggleSingleBlank(this)">비경쟁성</button> 때문에 <button type="button" class="blank-chip" data-term="무임승차자" onclick="toggleSingleBlank(this)">무임승차자</button> 문제가 발생해 시장에서 과소 공급됩니다.</li>
            <li><strong>ESG 경영</strong>: 기업이 환경(E)·사회(S)·지배구조(G)를 고려해 지속 가능 발전을 추구합니다.</li>
          </ul>

          <div class="table-wrap">
            <table class="clean-table">
              <thead>
                <tr>
                  <th>구분</th>
                  <th>대표 사례</th>
                  <th>시장 생산량</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td><strong>긍정적 외부효과</strong><br>(외부경제)</td>
                  <td>양봉업자 벌 사육 → 과수원 수확량 증가</td>
                  <td>사회적 적정량보다 <strong>적게</strong> 생산</td>
                </tr>
                <tr>
                  <td><strong>부정적 외부효과</strong><br>(외부불경제)</td>
                  <td>폐수 무단 방류, 공공장소 간접흡연</td>
                  <td>사회적 적정량보다 <strong>많이</strong> 생산</td>
                </tr>
              </tbody>
            </table>
          </div>
        </article>

        <!-- 카드 3: 세계화와 다국적 기업, 탄소 국경세 -->
        <article class="summary-card">
          <div class="hud-top">
            <span class="badge grape">단원 3 · 세계화와 평화</span>
            <span class="hud-label">입지·무역 핵심</span>
          </div>
          <h3 class="section-title">세계 도시 · 다국적 기업 · 탄소 국경세</h3>
          <ul class="summary-list">
            <li><strong>세계 도시</strong>: 세계 정치·경제·문화 중심지 역할을 하는 도시 (<button type="button" class="blank-chip" data-term="뉴욕·런던·도쿄·파리" onclick="toggleSingleBlank(this)">뉴욕·런던·도쿄·파리</button>).</li>
            <li><strong>자유 무역의 딜레마</strong>: 효율성과 선택 폭은 늘지만 취약 산업 위축 및 빈부·환경 격차를 유발합니다.</li>
            <li><strong><button type="button" class="blank-chip" data-term="탄소 국경세" onclick="toggleSingleBlank(this)">탄소 국경세</button></strong>: 탄소 규제가 약한 국가에서 강한 국가로 수출 시 추가 관세를 부과해 환경 덤핑을 막는 무역 장벽입니다.</li>
          </ul>

          <div class="table-wrap">
            <table class="clean-table">
              <thead>
                <tr>
                  <th>기업 기능</th>
                  <th>주요 입지 지역 및 이유</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td><strong>본사 (경영·기획)</strong></td>
                  <td>자본·정보가 집중된 대도시</td>
                </tr>
                <tr>
                  <td><strong>연구개발 (R&amp;D)</strong></td>
                  <td>연구 수준이 높고 우수 인재 확보가 쉬운 선진국</td>
                </tr>
                <tr>
                  <td><strong>생산 공장</strong></td>
                  <td>저임금 개발도상국 또는 무역 장벽 극복용 선진국</td>
                </tr>
              </tbody>
            </table>
          </div>
        </article>

        <!-- 카드 4: 기후 변화와 지속 가능한 발전, 정의와 인권 -->
        <article class="summary-card">
          <div class="hud-top">
            <span class="badge tangerine">단원 4 · 지속가능성 &amp; 정의</span>
            <span class="hud-label">주체별 실천</span>
          </div>
          <h3 class="section-title">기후 불평등 대응과 정의의 기준</h3>
          <ul class="summary-list">
            <li><strong>기후변화 특성과 영향</strong>: 화석 에너지 사용 등 <button type="button" class="blank-chip" data-term="인위적 요인" onclick="toggleSingleBlank(this)">인위적 요인</button>이 크며, 이상 기후와 해수면 상승뿐 아니라 지역·세대·계층 간 <button type="button" class="blank-chip" data-term="불평등 심화" onclick="toggleSingleBlank(this)">불평등 심화</button>를 초래합니다.</li>
            <li><strong>국제 사회</strong>: 기후변화 협약 체결, 개발도상국에 대한 재정·기술적 지원.</li>
            <li><strong>국가</strong>: 탄소 중립 정책, <button type="button" class="blank-chip" data-term="탄소배출권 거래제도" onclick="toggleSingleBlank(this)">탄소배출권 거래제도</button>, 신재생 에너지 공급 정책.</li>
            <li><strong>개인</strong>: 저탄소 친환경 제품 소비, 자원 절약 및 재활용, 윤리적 소비.</li>
            <li><strong>분배적·교정적 정의</strong>: 업적·필요·능력에 따른 공정한 분배(<button type="button" class="blank-chip" data-term="분배적 정의" onclick="toggleSingleBlank(this)">분배적 정의</button>)와 불법·피해 회복(<button type="button" class="blank-chip" data-term="교정적 정의" onclick="toggleSingleBlank(this)">교정적 정의</button>).</li>
          </ul>

          <div class="trap-callout">
            <i data-lucide="alert-triangle" aria-hidden="true" width="18" height="18" style="flex-shrink:0;"></i>
            <div><strong>1등급 함정 주의!</strong><br>환불 불가능한 예매권(매몰비용)과 알바를 빠져 포기한 임금(암묵적 비용)을 혼동하지 마세요. 매몰비용은 계산에서 반드시 제외해야 합니다!</div>
          </div>
        </article>
      </div>
    </section>

  </main>

  <footer class="source-note">
    출처 안내: 본 애플리케이션의 모든 문제·플래시카드·요약 내용은 고등학교 1학년 통합사회2 기말고사 대비 학습 노트 및 핵심 교과 개념을 바탕으로 제작되었습니다.
  </footer>

  <api-shim></api-shim>
  <script>
    const UNIT_LABELS = {
      market: `시장경제·합리적 선택`,
      global: `세계화·국제무역`,
      climate: `기후변화·지속가능`,
      justice: `정의와 인권`
    };

    const FLASHCARDS = [
      {
        id: `fc-1`,
        unit: `market`,
        term: `합리적 선택`,
        question: `비용과 편익을 비교해 선택할 때 반드시 충족해야 하는 조건은 무엇인가요?`,
        answer: `최소의 비용으로 최대의 편익을 얻는 선택으로, 반드시 '편익 > 기회비용(명시적 비용 + 암묵적 비용)'이어야 합리적 선택이 됩니다.`,
        tip: `같은 편익이면 최소 비용, 같은 비용이면 최대 편익을 선택!`
      },
      {
        id: `fc-2`,
        unit: `market`,
        term: `기회비용`,
        question: `어떤 선택을 할 때 포기해야 하는 대안의 가치를 포함한 총비용은 어떻게 구성되나요?`,
        answer: `실제로 화폐를 지출하는 '명시적 비용'과 선택으로 인해 포기한 소득이나 가치인 '암묵적 비용'을 더하여 계산합니다.`,
        tip: `티켓 가격(명시적) + 빠진 알바 시급(암묵적) 합산을 잊지 마세요.`
      },
      {
        id: `fc-3`,
        unit: `market`,
        term: `매몰비용 (Sunk Cost)`,
        question: `이미 지불하여 돌이킬 수 없는 비용을 합리적 의사결정에서 어떻게 처리해야 할까요?`,
        answer: `이미 지출되어 회수할 수 없는 비용이므로, 이후의 합리적 의사결정에서는 전적으로 배제해야 합니다.`,
        tip: `환불 불가 티켓·이미 낸 입장료는 절대 기회비용에 넣지 마세요!`
      },
      {
        id: `fc-4`,
        unit: `market`,
        term: `시장 실패`,
        question: `시장 기구가 자원을 효율적으로 배분하지 못하는 현상과 3가지 대표 원인은?`,
        answer: `시장에 맡겼을 때 적정량이 생산·분배되지 못하는 상태로, 대표적으로 독과점, 공공재 공급 부족, 외부효과가 있습니다.`,
        tip: `정부의 개입(규제, 공공재 직접 공급, 조세·보조금)이 필요한 이유입니다.`
      },
      {
        id: `fc-5`,
        unit: `market`,
        term: `독과점`,
        question: `소수의 기업이 시장을 지배할 때 소비자와 자원 배분에 어떤 문제가 생기나요?`,
        answer: `소수 공급자가 가격이나 공급량을 임의로 조절하여 소비자가 높은 가격에 구매하게 되고, 자원이 비효율적으로 배분됩니다.`,
        tip: `공정거래위원회의 담합 규제 및 독점 규제 대상입니다.`
      },
      {
        id: `fc-6`,
        unit: `market`,
        term: `공공재 (비배제성·비경쟁성)`,
        question: `가로등·국방 같은 공공재가 시장에서 충분히 공급되지 않는 두 가지 핵심 특성은?`,
        answer: `대가를 내지 않아도 소비를 막을 수 없는 '비배제성'과 한 사람의 소비가 타인의 소비량을 줄이지 않는 '비경쟁성'으로 인해 무임승차자 문제가 발생합니다.`,
        tip: `무임승차 문제 때문에 기업이 생산을 기피해 정부가 직접 공급합니다.`
      },
      {
        id: `fc-7`,
        unit: `market`,
        term: `긍정적 외부효과 (외부경제)`,
        question: `타인에게 의도치 않은 혜택을 주면서도 대가를 받지 못할 때 시장 생산량은 어떻게 되나요?`,
        answer: `대가(보상)를 받지 못하기 때문에 사회적으로 필요한 적정량보다 적게(과소) 생산됩니다. 예: 양봉업자의 벌 사육 → 과수원 수확량 증가.`,
        tip: `정부는 보조금 지급·세제 혜택으로 생산을 장려합니다.`
      },
      {
        id: `fc-8`,
        unit: `market`,
        term: `부정적 외부효과 (외부불경제)`,
        question: `타인에게 의도치 않은 손해를 끼치면서 대가를 치르지 않을 때 시장 생산량은?`,
        answer: `피해 비용을 지불하지 않아 사회적으로 적정한 양보다 많이(과다) 생산됩니다. 예: 폐수 무단 방류, 공공장소 간접흡연.`,
        tip: `정부는 환경세 부과·배출 규제 등으로 생산을 줄이려 합니다.`
      },
      {
        id: `fc-9`,
        unit: `market`,
        term: `ESG 경영`,
        question: `기업이 지속 가능한 성장을 위해 재무적 성과 외에 고려해야 하는 3대 요소는?`,
        answer: `환경(Environment), 사회(Social), 지배구조(Governance)를 함께 고려하는 책임 있는 경영 방식입니다.`,
        tip: `탄소 절감, 노동 인권 보호, 투명한 이사회 운영이 대표 사례입니다.`
      },
      {
        id: `fc-10`,
        unit: `global`,
        term: `세계 도시`,
        question: `국가의 경계를 넘어 세계의 정치·경제·문화적 중심지 역할을 수행하는 도시는?`,
        answer: `초국적 기업 본사와 금융기관, 국제기구가 집중된 도시로 대표적으로 뉴욕, 런던, 도쿄, 파리 등이 있습니다.`,
        tip: `세계화 시대에 국가보다 도시 간 네트워크 연결이 강해집니다.`
      },
      {
        id: `fc-11`,
        unit: `global`,
        term: `다국적 기업의 공간적 분업`,
        question: `다국적 기업이 본사, 연구개발(R&D), 생산 공장을 서로 다른 지역에 배치하는 원리는?`,
        answer: `각 기능별로 가장 유리한 입지를 선택하는 현상입니다. 본사는 대도시, R&D는 우수 인재가 많은 선진국, 생산 공장은 임금이 저렴한 개발도상국(또는 무역 장벽 극복용 선진국)에 입지합니다.`,
        tip: `생산 공장이 선진국에 세워지는 이유 = 무역 장벽 극복 & 현지 시장 개척!`
      },
      {
        id: `fc-12`,
        unit: `global`,
        term: `탄소 국경세`,
        question: `유럽·미국 등이 추진하며 탄소 규제가 약한 국가의 수출품에 추가 부과하는 관세는?`,
        answer: `이산화탄소 배출 규제가 약한 국가에서 강한 국가로 상품·서비스를 수출할 때 추가로 부과하는 관세로, 환경 덤핑 방지 목적의 새로운 무역 장벽입니다.`,
        tip: `우리나라 수출 기업도 저탄소 생산 공정 전환이 필수적입니다.`
      },
      {
        id: `fc-13`,
        unit: `global`,
        term: `자유 무역의 딜레마`,
        question: `자유 무역 확대가 가져오는 혜택과 동시에 발생하는 그림자(문제점)는 무엇인가요?`,
        answer: `소비자 선택 폭 확대와 경제 효율성 증대라는 장점 이면에, 국내 경쟁력 약화 산업 위축, 국가·계층 간 빈부 격차 심화, 환경 규제 회피 등의 문제가 나타납니다.`,
        tip: `무역 이익의 공정한 분배와 피해 산업 보호 대책이 요구됩니다.`
      },
      {
        id: `fc-14`,
        unit: `climate`,
        term: `기후변화의 인위적 요인`,
        question: `오늘날 지구촌이 겪는 급격한 기후변화의 가장 결정적인 원인은 무엇인가요?`,
        answer: `산업화 이후 화석 에너지 사용 증가에 따른 온실가스(이산화탄소 등) 배출과 무분별한 삼림 파괴 등 인간의 활동(인위적 요인)이 결정적 영향을 미칩니다.`,
        tip: `이상 기후, 해수면 상승, 생태계 교란으로 이어집니다.`
      },
      {
        id: `fc-15`,
        unit: `climate`,
        term: `기후 불평등`,
        question: `기후변화의 피해가 온실가스 배출 책임과 무관하게 나타나는 불공정 현상은?`,
        answer: `기후변화로 인한 재해와 피해가 배출량이 적은 저개발국, 사회적 취약 계층, 미래 세대에게 집중되어 지역·세대·계층 간 불평등이 심화되는 현상입니다.`,
        tip: `기후 정의(Climate Justice) 관점에서 국제 협력이 필요합니다.`
      },
      {
        id: `fc-16`,
        unit: `climate`,
        term: `탄소배출권 거래제도`,
        question: `국가가 기업에게 온실가스 배출 허용량을 정해주고 남거나 부족한 양을 거래하게 하는 제도는?`,
        answer: `기업에 배출 허용량을 할당하고 시장에서 배출권을 사고팔 수 있게 하여 기업 스스로 온실가스를 감축하도록 유도하는 국가 차원의 정책입니다.`,
        tip: `주체 구분 주의: '국가' 차원의 지속 가능 발전 정책입니다.`
      },
      {
        id: `fc-17`,
        unit: `climate`,
        term: `탄소 중립 (Net-Zero)`,
        question: `온실가스 순배출량을 실질적으로 '0'으로 만드는 환경 목표는 무엇인가요?`,
        answer: `온실가스 배출을 최대한 줄이고, 남은 배출량은 산림이나 기술로 흡수·제거하여 실질적 배출량을 0으로 맞추는 상태입니다.`,
        tip: `국가 차원의 탄소 중립 선언과 신재생 에너지 확대 정책으로 추진됩니다.`
      },
      {
        id: `fc-18`,
        unit: `justice`,
        term: `분배적 정의 vs 교정적 정의`,
        question: `사회적 가치 배분과 불법·부당 행위 바로잡기는 각각 어떤 정의에 해당하나요?`,
        answer: `업적·필요·능력 등의 기준에 따라 자원과 기회를 공정하게 나누는 것은 '분배적 정의', 불법 행위나 불균형을 처벌·배상으로 바로잡는 것은 '교정적 정의'입니다.`,
        tip: `필요에 따른 분배는 약자 보호에 강하지만 근로 의욕 저하 우려가 있습니다.`
      }
    ];

    const QUIZ_BANK = [
      {
        id: `q-1`,
        unit: `market`,
        tag: `기회비용 계산`,
        difficulty: `1등급 킬러`,
        question: `주은이의 영화 관람이 합리적 선택이 되려면 영화 관람에 따른 최소한의 편익은 얼마보다 커야 하는가?`,
        context: `[보기] 주은이는 시급 11,000원을 받으며 하루 4시간씩 카페에서 아르바이트를 하고 있다. 좋아하는 배우의 영화 무대 인사를 보러 가기 위해 30,000원을 내고 표를 구매했다. 단, 약속 시간이 아르바이트와 겹쳐 영화를 보려면 아르바이트 2시간을 빼야 한다. (표값 외 지출 없음)`,
        options: [
          `22,000원 초과`,
          `30,000원 초과`,
          `52,000원 초과`,
          `66,000원 초과`
        ],
        answerIndex: 2,
        explanation: `합리적 선택이 되려면 '편익 > 기회비용'이어야 합니다. 명시적 비용(실제 지출한 표값 30,000원) + 암묵적 비용(포기한 알바 2시간 임금 11,000원 × 2 = 22,000원) = 총 기회비용 52,000원! 따라서 편익이 52,000원을 초과해야 합니다.`
      },
      {
        id: `q-2`,
        unit: `market`,
        tag: `매몰비용 함정`,
        difficulty: `1등급 변별력`,
        question: `환불이 불가능한 콘서트 티켓을 10만 원에 예매했으나, 당일 고열과 몸살이 났다. 이때 합리적 의사결정 태도로 가장 옳은 것은?`,
        context: ``,
        options: [
          `이미 낸 10만 원이 아까우므로 무조건 콘서트장에 간다.`,
          `이미 지출해 회수할 수 없는 10만 원(매몰비용)은 배제하고, 앞으로 얻을 편익과 건강 손실 비용만 따져 결정한다.`,
          `콘서트 티켓 가격 10만 원에 병원비까지 더해 암묵적 비용으로 계산한다.`,
          `친구에게 티켓을 양도하지 못하면 합리적 선택 자체가 불가능하다.`
        ],
        answerIndex: 1,
        explanation: `이미 지불하여 회수할 수 없는 비용은 '매몰비용'입니다. 합리적인 의사결정을 할 때는 매몰비용을 전적으로 배제하고, 선택 시점 이후에 발생할 편익과 기회비용만을 비교해야 합니다.`
      },
      {
        id: `q-3`,
        unit: `market`,
        tag: `공공재 특성`,
        difficulty: `기출 핵심`,
        question: `국방, 치안, 가로등과 같은 공공재가 시장에만 맡겨지면 사회적으로 필요한 만큼 충분히 공급되지 못하는 핵심 이유 두 가지는?`,
        context: ``,
        options: [
          `배제성과 경합성`,
          `비배제성과 비경쟁성`,
          `수익성과 독점성`,
          `외부경제와 매몰비용`
        ],
        answerIndex: 1,
        explanation: `공공재는 대가를 내지 않은 사람의 소비를 막을 수 없는 '비배제성'과, 한 사람이 소비해도 타인의 소비량이 줄지 않는 '비경쟁성(비경합성)'을 지녀 무임승차자 문제가 발생합니다. 이로 인해 시장에서 충분히 공급되지 못합니다.`
      },
      {
        id: `q-4`,
        unit: `market`,
        tag: `긍정적 외부효과`,
        difficulty: `기출 핵심`,
        question: `다음 중 '긍정적 외부효과(외부경제)'의 사례로 가장 옳은 것은?`,
        context: ``,
        options: [
          `어떤 기업이 폐수를 무단 방류하여 인근 어민들이 피해를 보았다.`,
          `양봉업자가 꿀을 얻기 위해 벌을 키웠더니, 인근 과수원의 과일 수확량이 늘어났다.`,
          `흡연자가 공공장소에서 흡연하여 비흡연자들이 간접흡연 피해를 겪었다.`,
          `소수 독과점 기업이 공급량을 줄여 소비자가 비싼 가격에 물건을 샀다.`
        ],
        answerIndex: 1,
        explanation: `양봉업자의 꿀 생산 행위가 과수원 주인에게 의도하지 않은 혜택(수확량 증가)을 주면서도 대가를 받지 않으므로 '긍정적 외부효과'입니다. ①·③은 부정적 외부효과, ④는 독과점 문제입니다.`
      },
      {
        id: `q-5`,
        unit: `market`,
        tag: `외부효과 생산량`,
        difficulty: `1등급 변별력`,
        question: `외부효과가 시장에 방치될 경우, 사회적 최적 생산량과 비교한 실제 시장 생산량의 모습으로 옳게 짝지어진 것은?`,
        context: ``,
        options: [
          `긍정적 외부효과: 과다 생산 / 부정적 외부효과: 과소 생산`,
          `긍정적 외부효과: 과소 생산 / 부정적 외부효과: 과다 생산`,
          `긍정적 외부효과: 적정 생산 / 부정적 외부효과: 과소 생산`,
          `둘 다 사회적으로 필요한 양보다 과소 생산된다.`
        ],
        answerIndex: 1,
        explanation: `긍정적 외부효과는 혜택에 대한 보상을 못 받아 사회 적정량보다 '적게(과소)' 생산되고, 부정적 외부효과는 피해 비용을 치르지 않아 사회 적정량보다 '많이(과다)' 생산됩니다.`
      },
      {
        id: `q-6`,
        unit: `market`,
        tag: `독과점 시장`,
        difficulty: `기출 기본`,
        question: `시장 실패 원인 중 '독과점'이 발생했을 때 나타나는 결과에 대한 설명으로 옳은 것은?`,
        context: ``,
        options: [
          `기업 간 치열한 경쟁으로 상품 가격이 지나치게 폭락한다.`,
          `무임승차자 문제가 발생해 상품이 시장에서 완전히 사라진다.`,
          `소수의 공급자가 가격이나 공급량을 임의로 조절하여 자원이 비효율적으로 배분된다.`,
          `소비자들이 항상 최저 가격과 최고 품질의 상품을 누릴 수 있다.`
        ],
        answerIndex: 2,
        explanation: `독과점 시장에서는 소수 기업이 시장 지배력을 행사해 가격을 높이거나 공급량을 줄여 소비자의 후생이 감소하고 자원 배분의 비효율성이 발생합니다.`
      },
      {
        id: `q-7`,
        unit: `market`,
        tag: `ESG 경영`,
        difficulty: `기출 핵심`,
        question: `오늘날 기업이 장기적·지속 가능한 발전을 위해 재무적 성과 외에 반드시 고려해야 할 'ESG 경영'의 세 가지 축이 바르게 연결된 것은?`,
        context: ``,
        options: [
          `경제(Economy) · 과학(Science) · 성장(Growth)`,
          `환경(Environment) · 사회(Social) · 지배구조(Governance)`,
          `효율(Efficiency) · 안전(Safety) · 세계화(Globalization)`,
          `수출(Export) · 저축(Saving) · 정부(Government)`
        ],
        answerIndex: 1,
        explanation: `ESG 경영은 환경(Environment), 사회(Social), 지배구조(Governance)를 뜻하며, 기업의 윤리적·사회적 책임을 강조하는 핵심 경영 패러다임입니다.`
      },
      {
        id: `q-8`,
        unit: `global`,
        tag: `탄소 국경세`,
        difficulty: `1등급 변별력`,
        question: `유럽과 미국 등이 도입을 추진하는 '탄소 국경세'에 대한 설명으로 가장 옳은 것은?`,
        context: ``,
        options: [
          `탄소 배출이 많은 국가에 국제 사회가 무상으로 지원금을 주는 제도이다.`,
          `이산화탄소 배출 규제가 약한 국가에서 강한 국가로 수출할 때 추가로 부과하는 관세로, 환경 덤핑을 막기 위한 것이다.`,
          `국내 소비자가 해외여행 시 지불하는 항공 유류할증료의 다른 이름이다.`,
          `개발도상국의 산업화를 돕기 위해 관세를 완전히 면제해 주는 협약이다.`
        ],
        answerIndex: 1,
        explanation: `탄소 국경세는 온실가스 배출 규제가 느슨한 나라에서 생산된 제품이 규제가 강한 나라로 수출될 때 추가 관세를 물려 환경 덤핑을 방지하고 공정 경쟁을 유도하는 새로운 무역 장벽입니다.`
      },
      {
        id: `q-9`,
        unit: `global`,
        tag: `공간적 분업 R&D`,
        difficulty: `기출 핵심`,
        question: `다국적 기업의 공간적 분업 과정에서 '연구개발(R&D) 기능'이 주로 입지하는 지역과 그 이유로 옳은 것은?`,
        context: ``,
        options: [
          `임금이 저렴하고 노동력이 풍부한 개발도상국`,
          `연구 수준이 높고 우수한 인재를 확보하기 쉬운 선진국`,
          `원자재 수송이 편리한 해안가 공업 단지`,
          `인구 밀도가 가장 낮은 극지방`
        ],
        answerIndex: 1,
        explanation: `다국적 기업의 본사는 대도시에, 연구개발(R&D) 기능은 연구 수준이 높고 우수 인재를 확보할 수 있는 선진국에 주로 입지합니다.`
      },
      {
        id: `q-10`,
        unit: `global`,
        tag: `생산공장 입지`,
        difficulty: `1등급 변별력`,
        question: `다국적 기업의 생산 공장은 주로 임금이 저렴한 개발도상국에 입지하지만, 때로는 선진국에도 세워진다. 생산 공장이 '선진국'에 입지하는 주된 이유는?`,
        context: ``,
        options: [
          `선진국의 임금 수준이 개발도상국보다 훨씬 낮기 때문이다.`,
          `선진국의 환경 규제가 전혀 없어 오염 물질 배출이 자유롭기 때문이다.`,
          `선진국의 무역 장벽(관세·수입 규제 등)을 극복하고 현지 시장을 공략하기 위해서이다.`,
          `연구개발(R&D) 인력과 단순 생산 인력을 동일시하기 때문이다.`
        ],
        answerIndex: 2,
        explanation: `생산 공장은 비용 절감을 위해 개발도상국에 주로 세우지만, 높은 관세나 수입 쿼터 같은 선진국의 무역 장벽을 피하고 소비 시장에 근접하기 위해 선진국 현지에 공장을 세우기도 합니다.`
      },
      {
        id: `q-11`,
        unit: `global`,
        tag: `세계 도시`,
        difficulty: `기출 기본`,
        question: `국가의 경계를 넘어 세계의 정치·경제·문화적 중심지 역할을 수행하는 대표적인 '세계 도시'들로 묶인 것은?`,
        context: ``,
        options: [
          `뉴욕, 런던, 도쿄, 파리`,
          `아테네, 카이로, 멕시코시티, 울란바토르`,
          `나이로비, 리마, 다카, 하노이`,
          `리스본, 오슬로, 헬싱키, 소피아`
        ],
        answerIndex: 0,
        explanation: `뉴욕, 런던, 도쿄, 파리 등은 다국적 기업 본사, 국제 금융, 문화·정보 네트워크가 집중된 대표적 세계 도시입니다.`
      },
      {
        id: `q-12`,
        unit: `climate`,
        tag: `기후변화 영향`,
        difficulty: `기출 핵심`,
        question: `오늘날 진행되는 기후변화의 원인과 영향에 대한 설명으로 옳지 않은 것은?`,
        context: ``,
        options: [
          `화석 에너지 사용 증가에 따른 온실가스 배출 등 인위적 요인의 영향이 크다.`,
          `이상 기후, 해수면 상승, 생태계 교란 등 다양한 환경 문제가 발생한다.`,
          `기후변화로 인한 피해는 전 세계 모든 지역·세대·계층에게 똑같이 평등하게 나타난다.`,
          `온실가스를 적게 배출한 저개발국이나 취약 계층이 더 큰 피해를 입는 기후 불평등이 심화된다.`
        ],
        answerIndex: 2,
        explanation: `기후변화의 영향은 동일하게 나타나지 않으며, 대응 역량이 부족한 저개발국·취약 계층·미래 세대에 피해가 집중되어 지역·세대·계층 간 불평등을 심화시킵니다.`
      },
      {
        id: `q-13`,
        unit: `climate`,
        tag: `주체별 대응 방안`,
        difficulty: `기출 핵심`,
        question: `지속 가능한 발전을 위한 노력 중 '국가' 차원의 정책으로 가장 적절한 것은?`,
        context: ``,
        options: [
          `개발도상국에 대한 국제적 재정·기술 지원 협정 체결`,
          `탄소 중립 정책 마련, 탄소배출권 거래제도, 신재생 에너지 공급 정책`,
          `개인의 저탄소 친환경 제품 구매 및 분리배출 실천`,
          `비정부 기구(NGO)의 국경 간 환경 감시 캠페인`
        ],
        answerIndex: 1,
        explanation: `탄소 중립 정책, 탄소배출권 거래제도, 신재생 에너지 공급 정책은 '국가' 차원의 대표적 실천 방안입니다. ①은 국제 사회, ③은 개인 차원의 노력입니다.`
      },
      {
        id: `q-14`,
        unit: `global`,
        tag: `자유 무역 딜레마`,
        difficulty: `1등급 변별력`,
        question: `자유 무역의 확대가 가져오는 양면성(자유 무역의 딜레마)에 대한 설명으로 가장 적절한 것은?`,
        context: ``,
        options: [
          `모든 국가의 모든 산업이 예외 없이 동시에 성장한다.`,
          `소비자의 선택 폭과 효율성은 늘지만, 경쟁력이 약한 국내 산업 위축과 국가·계층 간 격차가 심화될 수 있다.`,
          `자유 무역은 환경 오염을 자동으로 100% 해결해 준다.`,
          `관세가 사라지면 다국적 기업의 공간적 분업은 완전히 중단된다.`
        ],
        answerIndex: 1,
        explanation: `자유 무역은 전체 부의 증대와 소비자 후생 증가라는 이익을 주지만, 국내 취약 산업 위축과 분배 불평등·환경 덤핑이라는 딜레마를 동반합니다.`
      },
      {
        id: `q-15`,
        unit: `justice`,
        tag: `분배적 정의 기준`,
        difficulty: `기출 핵심`,
        question: `분배적 정의의 실질적 기준 중 '필요에 따른 분배'가 갖는 장단점을 바르게 설명한 것은?`,
        context: ``,
        options: [
          `개인의 노력에 비례해 보상하므로 근로 의욕이 극대화된다.`,
          `사회적 약자를 보호해 인간다운 삶을 보장할 수 있으나, 개인의 성취·근로 의욕이 저하될 수 있다.`,
          `재능이 뛰어난 사람에게만 자원이 쏠려 사회적 약자가 방치된다.`,
          `누구에게나 무조건 똑같은 양을 나누어 개인 차를 무시한다.`
        ],
        answerIndex: 1,
        explanation: `'필요'에 따른 분배는 인간다운 삶과 사회 안전망 보장에 유리하지만, 노력과 기여에 상관없이 분배될 경우 근로 의욕이 떨어질 수 있는 한계가 있습니다.`
      },
      {
        id: `q-16`,
        unit: `market`,
        tag: `종합 킬러 문항`,
        difficulty: `1등급 최고난도`,
        question: `민수가 합리적 선택을 한다면 어떤 결정을 내려야 하며, 그 근거로 옳은 것은?`,
        context: `[보기] 민수는 15,000원을 내고 환불이 불가능한 전시회 예매권을 샀다. 그런데 전시회 당일 같은 시간에 시급 12,000원짜리 단기 아르바이트(2시간) 제안을 받았다. 민수가 전시회를 관람할 때 얻는 주관적 편익은 20,000원이다.`,
        options: [
          `전시회를 본다. (편익 20,000원 > 티켓값 15,000원)`,
          `전시회를 본다. (총 편익이 39,000원을 넘기 때문)`,
          `전시회를 포기하고 아르바이트를 한다. (매몰비용 15,000원 배제 시, 편익 20,000원 < 포기한 알바 임금 24,000원)`,
          `전시회를 포기한다. (매몰비용 15,000원 + 알바비 24,000원 = 39,000원 손해이므로)`
        ],
        answerIndex: 2,
        explanation: `최고난도 함정 문제입니다! 이미 지불한 환불 불가 예매권 15,000원은 '매몰비용'이므로 반드시 배제합니다. 전시회 선택 시 포기하는 암묵적 기회비용은 알바 2시간 임금 24,000원(12,000 × 2)입니다. 전시회 편익(20,000원)이 기회비용(24,000원)보다 작으므로 아르바이트를 선택하는 것이 합리적입니다!`
      }
    ];

    let appState = {
      towerFloor: 0,
      bestFloor: 0,
      score: 0,
      streak: 0,
      bestStreak: 0,
      solvedIds: [],
      wrongIds: [],
      masteredCardIds: [],
      towerBlocks: [],
      activeMode: `tower`,
      activeQuizFilter: `all`,
      activeCardFilter: `all`,
      blankMode: false
    };

    let currentQuizIndex = 0;
    let currentFilteredQuizzes = QUIZ_BANK.slice();
    let currentQuizAnswered = false;
    let lastEventType = `neutral`;
    let lastEventText = `정답 시 +1층 & +100점(콤보 보너스), 오답 시 -1층 & -50점 감점됩니다.`;

    let currentCardIndex = 0;
    let currentFilteredCards = FLASHCARDS.slice();
    let isCardFlipped = false;

    function refreshIcons() {
      if (typeof lucide !== `undefined` && typeof lucide.createIcons === `function`) {
        lucide.createIcons();
      }
    }

    async function saveAppState() {
      try {
        if (window.notebookAppApi && typeof window.notebookAppApi.setAppState === `function`) {
          await window.notebookAppApi.setAppState(appState);
        }
      } catch (e) {
        // Ignore transient host persistence error
      }
    }

    async function initApp() {
      try {
        if (window.notebookAppApi && typeof window.notebookAppApi.getAppState === `function`) {
          const saved = await window.notebookAppApi.getAppState();
          if (saved && typeof saved === `object`) {
            appState = {
              ...appState,
              ...saved,
              solvedIds: Array.isArray(saved.solvedIds) ? saved.solvedIds : [],
              wrongIds: Array.isArray(saved.wrongIds) ? saved.wrongIds : [],
              masteredCardIds: Array.isArray(saved.masteredCardIds) ? saved.masteredCardIds : [],
              towerBlocks: Array.isArray(saved.towerBlocks) ? saved.towerBlocks : []
            };
          }
        }
      } catch (e) {
        // Fallback to clean initial state
      }

      if (appState.blankMode) {
        applyBlankModeUI();
      }
      applyQuizFilterList();
      applyCardFilterList();
      switchMode(appState.activeMode || `tower`, true);
      renderAll();

      if (window.notebookAppApi && typeof window.notebookAppApi.notifyAppReady === `function`) {
        window.notebookAppApi.notifyAppReady();
      }
    }

    function renderAll() {
      renderHud();
      renderTower();
      renderQuiz();
      renderFlashcard();
      updateCostCalc();
      refreshIcons();
    }

    function renderHud() {
      const floorEl = document.getElementById(`hud-floor`);
      const floorSubEl = document.getElementById(`hud-floor-sub`);
      const floorBarEl = document.getElementById(`hud-floor-bar`);
      const scoreEl = document.getElementById(`hud-score`);
      const streakEl = document.getElementById(`hud-streak`);
      const cardsEl = document.getElementById(`hud-cards`);
      const cardsSubEl = document.getElementById(`hud-cards-sub`);
      const cardsBarEl = document.getElementById(`hud-cards-bar`);
      const bestEl = document.getElementById(`hud-best`);
      const wrongEl = document.getElementById(`hud-wrong`);
      const wrongFilterBtn = document.getElementById(`btn-wrong-filter`);
      const victoryBanner = document.getElementById(`victory-banner`);

      const pctFloor = Math.min(100, Math.round((appState.towerFloor / 15) * 100));
      const masteredCount = appState.masteredCardIds.length;
      const pctCards = Math.round((masteredCount / FLASHCARDS.length) * 100);

      if (floorEl) floorEl.textContent = `${appState.towerFloor}F`;
      if (floorSubEl) {
        floorSubEl.textContent = appState.towerFloor >= 15
          ? `15F 완공 달성! (1등급 마스터)`
          : `목표 15F까지 ${Math.max(0, 15 - appState.towerFloor)}층 남음`;
      }
      if (floorBarEl) floorBarEl.style.width = `${pctFloor}%`;
      if (scoreEl) scoreEl.textContent = `${appState.score.toLocaleString()}점`;
      if (streakEl) streakEl.textContent = `연속 정답 ${appState.streak}콤보 · 최고 ${appState.bestStreak}콤보`;
      if (cardsEl) cardsEl.textContent = `${masteredCount} / ${FLASHCARDS.length}`;
      if (cardsSubEl) cardsSubEl.textContent = `플래시카드 완성도 ${pctCards}%`;
      if (cardsBarEl) cardsBarEl.style.width = `${pctCards}%`;
      if (bestEl) bestEl.textContent = `최고 ${appState.bestFloor}F`;
      if (wrongEl) wrongEl.textContent = `오답 노트 ${appState.wrongIds.length}문항`;
      if (wrongFilterBtn) wrongFilterBtn.textContent = `오답 집중 복습 (${appState.wrongIds.length})`;
      if (victoryBanner) {
        victoryBanner.style.display = appState.towerFloor >= 15 ? `flex` : `none`;
      }
    }

    function switchMode(mode, skipSave) {
      appState.activeMode = mode;
      const modes = [`tower`, `flashcard`, `summary`];
      modes.forEach(function (m) {
        const tab = document.getElementById(`tab-${m}`);
        const panel = document.getElementById(`panel-${m}`);
        const isActive = m === mode;
        if (tab) {
          tab.classList.toggle(`active`, isActive);
          tab.setAttribute(`aria-selected`, isActive ? `true` : `false`);
        }
        if (panel) {
          panel.classList.toggle(`active`, isActive);
        }
      });
      if (!skipSave) {
        saveAppState();
      }
      refreshIcons();
    }

    /* ========================================
       TOWER RENDERING & QUIZ ENGINE
       ======================================== */
    function getTowerRankInfo(floor) {
      if (floor >= 15) return { rank: `1등급 마스터 타워 (${floor}F)`, next: `최고 기록 경신 중!` };
      if (floor >= 10) return { rank: `실버 2등급 타워 (${floor}F)`, next: `다음 목표: 15F 1등급 완공` };
      if (floor >= 5) return { rank: `브론즈 3등급 타워 (${floor}F)`, next: `다음 목표: 10F 실버 타워` };
      if (floor >= 1) return { rank: `초석 쌓기 (${floor}F)`, next: `다음 목표: 5F 브론즈 타워` };
      return { rank: `기초 공사 중 (0F)`, next: `다음 목표: 5F 브론즈 타워` };
    }

    function renderTower(animateCrumble) {
      const stackEl = document.getElementById(`tower-stack`);
      const rankEl = document.getElementById(`tower-rank-label`);
      const goalEl = document.getElementById(`tower-next-goal`);
      const heightBadge = document.getElementById(`tower-height-badge`);
      const bannerEl = document.getElementById(`tower-event-banner`);

      const info = getTowerRankInfo(appState.towerFloor);
      if (rankEl) rankEl.textContent = `현재 등급: ${info.rank}`;
      if (goalEl) goalEl.textContent = info.next;
      if (heightBadge) heightBadge.textContent = `${appState.towerFloor} / 15층`;

      if (bannerEl) {
        bannerEl.className = `tower-event-banner`;
        if (lastEventType === `gain`) bannerEl.classList.add(`gain`);
        if (lastEventType === `loss`) bannerEl.classList.add(`loss`);
        const iconName = lastEventType === `gain` ? `trending-up` : (lastEventType === `loss` ? `trending-down` : `info`);
        bannerEl.innerHTML = `<i data-lucide="${iconName}" aria-hidden="true" width="16" height="16"></i><span>${lastEventText}</span>`;
      }

      if (!stackEl) return;

      if (appState.towerBlocks.length === 0) {
        stackEl.innerHTML = `<div class="tower-empty-hint">아직 쌓인 블록이 없습니다.<br>오른쪽 첫 문제를 맞혀 1층 블록을 쌓아보세요!</div>`;
        return;
      }

      const blocksToShow = appState.towerBlocks.slice(-15);
      const hiddenCount = Math.max(0, appState.towerBlocks.length - blocksToShow.length);
      let html = ``;
      blocksToShow.forEach(function (blk, idx) {
        const isTop = idx === blocksToShow.length - 1;
        const crumbleCls = (animateCrumble && isTop) ? ` crumbling` : ``;
        html += `<div class="tower-block unit-${blk.unit}${crumbleCls}">
          <span><strong>${blk.floor}F</strong> · ${blk.tag}</span>
          <span>${UNIT_LABELS[blk.unit] || `핵심`}</span>
        </div>`;
      });
      if (hiddenCount > 0) {
        html = `<div class="tower-block unit-market"><span>1F ~ ${hiddenCount}F 하단 기초 층수 포함</span><span>+${hiddenCount}층</span></div>` + html;
      }
      stackEl.innerHTML = html;
    }

    function applyQuizFilterList() {
      const f = appState.activeQuizFilter;
      if (f === `all`) {
        currentFilteredQuizzes = QUIZ_BANK.slice();
      } else if (f === `wrong`) {
        currentFilteredQuizzes = QUIZ_BANK.filter(function (q) {
          return appState.wrongIds.indexOf(q.id) !== -1;
        });
      } else {
        currentFilteredQuizzes = QUIZ_BANK.filter(function (q) {
          return q.unit === f;
        });
      }
      if (currentQuizIndex >= currentFilteredQuizzes.length) {
        currentQuizIndex = 0;
      }
    }

    function setQuizFilter(filterVal) {
      appState.activeQuizFilter = filterVal;
      currentQuizIndex = 0;
      currentQuizAnswered = false;
      applyQuizFilterList();

      const chips = document.querySelectorAll(`[data-quiz-filter]`);
      chips.forEach(function (btn) {
        btn.classList.toggle(`active`, btn.getAttribute(`data-quiz-filter`) === filterVal);
      });

      saveAppState();
      renderQuiz();
      refreshIcons();
    }

    function renderQuiz() {
      const unitBadge = document.getElementById(`quiz-unit-badge`);
      const diffBadge = document.getElementById(`quiz-diff-badge`);
      const counterEl = document.getElementById(`quiz-counter`);
      const questionEl = document.getElementById(`quiz-question`);
      const contextEl = document.getElementById(`quiz-context`);
      const optionsEl = document.getElementById(`quiz-options`);
      const expBox = document.getElementById(`quiz-explanation`);
      const nextBtn = document.getElementById(`btn-next-question`);

      if (!questionEl || !optionsEl) return;

      if (currentFilteredQuizzes.length === 0) {
        if (unitBadge) unitBadge.textContent = `오답 복습 완료`;
        if (diffBadge) diffBadge.textContent = `완벽해요`;
        if (counterEl) counterEl.textContent = `0 / 0`;
        questionEl.textContent = `현재 오답 노트에 저장된 문항이 없습니다!`;
        if (contextEl) contextEl.style.display = `none`;
        optionsEl.innerHTML = `<button type="button" class="btn btn-primary" onclick="setQuizFilter('all')">전체 범위 문제로 돌아가기</button>`;
        if (expBox) expBox.style.display = `none`;
        if (nextBtn) nextBtn.disabled = true;
        return;
      }

      const q = currentFilteredQuizzes[currentQuizIndex];
      currentQuizAnswered = false;

      if (unitBadge) unitBadge.textContent = UNIT_LABELS[q.unit] || `통합사회`;
      if (diffBadge) diffBadge.textContent = q.difficulty;
      if (counterEl) counterEl.textContent = `문제 ${currentQuizIndex + 1} / ${currentFilteredQuizzes.length}`;
      questionEl.textContent = q.question;

      if (contextEl) {
        if (q.context && q.context.trim().length > 0) {
          contextEl.style.display = `block`;
          contextEl.textContent = q.context;
        } else {
          contextEl.style.display = `none`;
        }
      }

      const nums = [`①`, `②`, `③`, `④`];
      let optHtml = ``;
      q.options.forEach(function (optText, idx) {
        optHtml += `<button type="button" class="option-btn" data-opt-idx="${idx}" onclick="submitAnswer(${idx})">
          <span class="option-num">${nums[idx]}</span>
          <span>${optText}</span>
        </button>`;
      });
      optionsEl.innerHTML = optHtml;

      if (expBox) {
        expBox.style.display = `none`;
        expBox.className = `explanation-box`;
      }
      if (nextBtn) nextBtn.disabled = true;
    }

    function submitAnswer(selectedIdx) {
      if (currentQuizAnswered || currentFilteredQuizzes.length === 0) return;
      currentQuizAnswered = true;

      const q = currentFilteredQuizzes[currentQuizIndex];
      const isCorrect = selectedIdx === q.answerIndex;
      const optionBtns = document.querySelectorAll(`#quiz-options .option-btn`);

      optionBtns.forEach(function (btn, idx) {
        btn.disabled = true;
        if (idx === q.answerIndex) {
          btn.classList.add(`correct`);
        } else if (idx === selectedIdx && !isCorrect) {
          btn.classList.add(`wrong`);
        }
      });

      const expBox = document.getElementById(`quiz-explanation`);
      const expTitle = document.getElementById(`exp-title`);
      const expBody = document.getElementById(`exp-body`);
      const nextBtn = document.getElementById(`btn-next-question`);

      if (isCorrect) {
        appState.streak += 1;
        if (appState.streak > appState.bestStreak) appState.bestStreak = appState.streak;
        const comboBonus = Math.min(100, (appState.streak - 1) * 20);
        const gainedPoints = 100 + comboBonus;
        appState.score += gainedPoints;
        appState.towerFloor += 1;
        if (appState.towerFloor > appState.bestFloor) appState.bestFloor = appState.towerFloor;

        appState.towerBlocks.push({
          floor: appState.towerFloor,
          unit: q.unit,
          tag: q.tag
        });

        if (appState.solvedIds.indexOf(q.id) === -1) {
          appState.solvedIds.push(q.id);
        }
        const wrongPos = appState.wrongIds.indexOf(q.id);
        if (wrongPos !== -1) {
          appState.wrongIds.splice(wrongPos, 1);
        }

        lastEventType = `gain`;
        lastEventText = `정답! ${appState.towerFloor}층 블록 적립 (+${gainedPoints}점${comboBonus > 0 ? `, ${appState.streak}콤보 보너스` : ``})`;

        if (expBox && expTitle && expBody) {
          expBox.style.display = `flex`;
          expBox.classList.add(`is-correct`);
          expTitle.innerHTML = `<i data-lucide="check-circle-2" aria-hidden="true" width="20" height="20"></i> 정답입니다! (+1층 · +${gainedPoints}점)`;
          expBody.textContent = q.explanation;
        }
        renderTower(false);
      } else {
        appState.streak = 0;
        appState.score = Math.max(0, appState.score - 50);
        const prevFloor = appState.towerFloor;
        if (appState.towerFloor > 0) {
          appState.towerFloor -= 1;
          appState.towerBlocks.pop();
        }
        if (appState.wrongIds.indexOf(q.id) === -1) {
          appState.wrongIds.push(q.id);
        }

        lastEventType = `loss`;
        lastEventText = prevFloor > 0
          ? `오답! 탑의 최상단 블록이 깎였습니다 (${prevFloor}F → ${appState.towerFloor}F, -50점). 오답 노트에 저장됨.`
          : `오답! -50점 감점 및 오답 노트에 자동 저장되었습니다.`;

        if (expBox && expTitle && expBody) {
          expBox.style.display = `flex`;
          expBox.classList.add(`is-wrong`);
          expTitle.innerHTML = `<i data-lucide="x-circle" aria-hidden="true" width="20" height="20"></i> 아쉽습니다! 탑이 1층 깎였습니다 (-50점)`;
          expBody.textContent = q.explanation;
        }
        renderTower(true);
      }

      if (nextBtn) nextBtn.disabled = false;
      renderHud();
      saveAppState();
      refreshIcons();
    }

    function nextQuestion() {
      if (appState.activeQuizFilter === `wrong`) {
        applyQuizFilterList();
      }
      if (currentFilteredQuizzes.length > 0) {
        currentQuizIndex = (currentQuizIndex + 1) % currentFilteredQuizzes.length;
      }
      renderQuiz();
      refreshIcons();
    }

    function skipQuestion() {
      if (currentFilteredQuizzes.length > 1) {
        currentQuizIndex = (currentQuizIndex + 1) % currentFilteredQuizzes.length;
      }
      renderQuiz();
      refreshIcons();
    }

    function handleResetTower(btn) {
      if (!btn) return;
      if (btn.dataset.armed !== `true`) {
        btn.dataset.armed = `true`;
        btn.classList.remove(`btn-soft`);
        btn.classList.add(`btn-danger-soft`);
        btn.innerHTML = `<i data-lucide="alert-circle" aria-hidden="true" width="16" height="16"></i> 한 번 더 클릭해 초기화`;
        refreshIcons();
        setTimeout(function () {
          if (btn.dataset.armed === `true`) {
            btn.dataset.armed = `false`;
            btn.classList.remove(`btn-danger-soft`);
            btn.classList.add(`btn-soft`);
            btn.innerHTML = `<i data-lucide="rotate-ccw" aria-hidden="true" width="16" height="16"></i> 탑 초기화`;
            refreshIcons();
          }
        }, 4000);
        return;
      }

      btn.dataset.armed = `false`;
      btn.classList.remove(`btn-danger-soft`);
      btn.classList.add(`btn-soft`);
      btn.innerHTML = `<i data-lucide="rotate-ccw" aria-hidden="true" width="16" height="16"></i> 탑 초기화`;

      appState.towerFloor = 0;
      appState.streak = 0;
      appState.towerBlocks = [];
      lastEventType = `neutral`;
      lastEventText = `탑이 0F 기초 상태로 초기화되었습니다. 다시 도전해 보세요!`;

      renderHud();
      renderTower(false);
      saveAppState();
      refreshIcons();
    }

    /* ========================================
       FLASHCARD ENGINE
       ======================================== */
    function applyCardFilterList() {
      const f = appState.activeCardFilter;
      if (f === `all`) {
        currentFilteredCards = FLASHCARDS.slice();
      } else if (f === `unmastered`) {
        currentFilteredCards = FLASHCARDS.filter(function (c) {
          return appState.masteredCardIds.indexOf(c.id) === -1;
        });
      } else {
        currentFilteredCards = FLASHCARDS.filter(function (c) {
          return c.unit === f;
        });
      }
      if (currentCardIndex >= currentFilteredCards.length) {
        currentCardIndex = 0;
      }
    }

    function setCardFilter(filterVal) {
      appState.activeCardFilter = filterVal;
      currentCardIndex = 0;
      isCardFlipped = false;
      applyCardFilterList();

      const chips = document.querySelectorAll(`[data-card-filter]`);
      chips.forEach(function (btn) {
        btn.classList.toggle(`active`, btn.getAttribute(`data-card-filter`) === filterVal);
      });

      saveAppState();
      renderFlashcard();
      refreshIcons();
    }

    function renderFlashcard() {
      const cardBtn = document.getElementById(`flashcard-btn`);
      const unitFront = document.getElementById(`card-unit-front`);
      const termFront = document.getElementById(`card-term-front`);
      const qFront = document.getElementById(`card-question-front`);
      const termBack = document.getElementById(`card-term-back`);
      const aBack = document.getElementById(`card-answer-back`);
      const tipBack = document.getElementById(`card-tip-back`);
      const progLabel = document.getElementById(`flash-progress-label`);
      const progBar = document.getElementById(`flash-progress-bar`);
      const masteredBadge = document.getElementById(`flash-mastered-badge`);
      const dotsEl = document.getElementById(`term-dots`);

      if (cardBtn) {
        cardBtn.classList.toggle(`flipped`, isCardFlipped);
      }

      const masteredPct = Math.round((appState.masteredCardIds.length / FLASHCARDS.length) * 100);
      if (progBar) progBar.style.width = `${masteredPct}%`;

      if (currentFilteredCards.length === 0) {
        if (progLabel) progLabel.textContent = `모든 카드를 완벽히 암기했습니다! (암기율 100%)`;
        if (unitFront) unitFront.textContent = `완료`;
        if (termFront) termFront.textContent = `모든 용어 암기 완료!`;
        if (qFront) qFront.textContent = `상단 필터에서 '전체'를 누르면 모든 카드를 다시 복습할 수 있습니다.`;
        if (termBack) termBack.textContent = `1등급 준비 완료`;
        if (aBack) aBack.textContent = `18개 핵심 용어를 모두 마스터했습니다. 이제 '지식의 탑 퀴즈'에서 실력을 테스트해 보세요!`;
        if (tipBack) tipBack.textContent = ``;
        if (masteredBadge) masteredBadge.style.display = `inline-flex`;
        if (dotsEl) dotsEl.innerHTML = ``;
        return;
      }

      const c = currentFilteredCards[currentCardIndex];
      const isMastered = appState.masteredCardIds.indexOf(c.id) !== -1;

      if (progLabel) {
        progLabel.textContent = `현재 카드 ${currentCardIndex + 1} / ${currentFilteredCards.length} · 전체 암기율 ${masteredPct}%`;
      }
      if (masteredBadge) {
        masteredBadge.style.display = isMastered ? `inline-flex` : `none`;
      }
      if (unitFront) unitFront.textContent = UNIT_LABELS[c.unit] || `핵심`;
      if (termFront) termFront.textContent = c.term;
      if (qFront) qFront.textContent = c.question;
      if (termBack) termBack.textContent = c.term;
      if (aBack) aBack.textContent = c.answer;
      if (tipBack) tipBack.textContent = `💡 ${c.tip}`;

      if (dotsEl) {
        let dotsHtml = ``;
        currentFilteredCards.forEach(function (item, idx) {
          const mCls = appState.masteredCardIds.indexOf(item.id) !== -1 ? ` mastered` : ``;
          const cCls = idx === currentCardIndex ? ` current` : ``;
          dotsHtml += `<button type="button" class="term-pill${mCls}${cCls}" onclick="jumpToCard(${idx})">${item.term}</button>`;
        });
        dotsEl.innerHTML = dotsHtml;
      }
    }

    function flipFlashcard() {
      isCardFlipped = !isCardFlipped;
      const cardBtn = document.getElementById(`flashcard-btn`);
      if (cardBtn) cardBtn.classList.toggle(`flipped`, isCardFlipped);
    }

    function jumpToCard(idx) {
      currentCardIndex = idx;
      isCardFlipped = false;
      renderFlashcard();
      refreshIcons();
    }

    function nextFlashcard() {
      if (currentFilteredCards.length === 0) return;
      currentCardIndex = (currentCardIndex + 1) % currentFilteredCards.length;
      isCardFlipped = false;
      renderFlashcard();
      refreshIcons();
    }

    function prevFlashcard() {
      if (currentFilteredCards.length === 0) return;
      currentCardIndex = (currentCardIndex - 1 + currentFilteredCards.length) % currentFilteredCards.length;
      isCardFlipped = false;
      renderFlashcard();
      refreshIcons();
    }

    function markCardMastered() {
      if (currentFilteredCards.length === 0) return;
      const c = currentFilteredCards[currentCardIndex];
      if (appState.masteredCardIds.indexOf(c.id) === -1) {
        appState.masteredCardIds.push(c.id);
        appState.score += 20;
      }
      if (appState.activeCardFilter === `unmastered`) {
        applyCardFilterList();
      } else if (currentFilteredCards.length > 1) {
        currentCardIndex = (currentCardIndex + 1) % currentFilteredCards.length;
      }
      isCardFlipped = false;
      renderHud();
      renderFlashcard();
      saveAppState();
      refreshIcons();
    }

    function markCardReview() {
      if (currentFilteredCards.length === 0) return;
      const c = currentFilteredCards[currentCardIndex];
      const pos = appState.masteredCardIds.indexOf(c.id);
      if (pos !== -1) {
        appState.masteredCardIds.splice(pos, 1);
      }
      if (currentFilteredCards.length > 1) {
        currentCardIndex = (currentCardIndex + 1) % currentFilteredCards.length;
      }
      isCardFlipped = false;
      renderHud();
      renderFlashcard();
      saveAppState();
      refreshIcons();
    }

    function shuffleCards() {
      for (let i = currentFilteredCards.length - 1; i > 0; i -= 1) {
        const j = Math.floor(Math.random() * (i + 1));
        const tmp = currentFilteredCards[i];
        currentFilteredCards[i] = currentFilteredCards[j];
        currentFilteredCards[j] = tmp;
      }
      currentCardIndex = 0;
      isCardFlipped = false;
      renderFlashcard();
      refreshIcons();
    }

    function handleResetCards(btn) {
      if (!btn) return;
      if (btn.dataset.armed !== `true`) {
        btn.dataset.armed = `true`;
        btn.textContent = `한 번 더 클릭해 초기화`;
        setTimeout(function () {
          if (btn.dataset.armed === `true`) {
            btn.dataset.armed = `false`;
            btn.innerHTML = `<i data-lucide="refresh-cw" aria-hidden="true" width="16" height="16"></i> 암기 초기화`;
            refreshIcons();
          }
        }, 4000);
        return;
      }
      btn.dataset.armed = `false`;
      btn.innerHTML = `<i data-lucide="refresh-cw" aria-hidden="true" width="16" height="16"></i> 암기 초기화`;
      appState.masteredCardIds = [];
      applyCardFilterList();
      isCardFlipped = false;
      renderHud();
      renderFlashcard();
      saveAppState();
      refreshIcons();
    }

    /* ========================================
       SUMMARY BLANK MODE & MINI CALCULATOR
       ======================================== */
    function applyBlankModeUI() {
      const btn = document.getElementById(`btn-blank-toggle`);
      const label = document.getElementById(`blank-toggle-label`);
      const blanks = document.querySelectorAll(`.blank-chip`);

      if (btn) btn.setAttribute(`aria-pressed`, appState.blankMode ? `true` : `false`);
      if (label) label.textContent = appState.blankMode ? `암기 가림막 ON` : `암기 가림막 OFF`;

      blanks.forEach(function (chip) {
        if (appState.blankMode) {
          chip.classList.add(`hidden-answer`);
          chip.textContent = `??? 확인`;
        } else {
          chip.classList.remove(`hidden-answer`);
          chip.textContent = chip.getAttribute(`data-term`) || ``;
        }
      });
    }

    function toggleBlankMode() {
      appState.blankMode = !appState.blankMode;
      applyBlankModeUI();
      saveAppState();
    }

    function toggleSingleBlank(chip) {
      if (!chip) return;
      if (chip.classList.contains(`hidden-answer`)) {
        chip.classList.remove(`hidden-answer`);
        chip.textContent = chip.getAttribute(`data-term`) || ``;
      } else if (appState.blankMode) {
        chip.classList.add(`hidden-answer`);
        chip.textContent = `??? 확인`;
      }
    }

    function revealAllBlanks() {
      appState.blankMode = false;
      applyBlankModeUI();
      saveAppState();
    }

    function updateCostCalc() {
      const expEl = document.getElementById(`calc-explicit`);
      const wageEl = document.getElementById(`calc-wage`);
      const hrsEl = document.getElementById(`calc-hours`);
      const outEl = document.getElementById(`calc-output`);
      if (!expEl || !wageEl || !hrsEl || !outEl) return;

      const explicit = Math.max(0, Number(expEl.value) || 0);
      const wage = Math.max(0, Number(wageEl.value) || 0);
      const hours = Math.max(0, Number(hrsEl.value) || 0);
      const implicit = wage * hours;
      const total = explicit + implicit;

      outEl.innerHTML = `<span>총 기회비용: <strong style="color: var(--primary);">${total.toLocaleString()}원</strong> (명시적 ${explicit.toLocaleString()} + 암묵적 ${implicit.toLocaleString()})</span>
        <span class="hud-label">편익이 ${total.toLocaleString()}원 초과 시 합리적 선택</span>`;
    }

    document.addEventListener(`keydown`, function (e) {
      if (appState.activeMode === `flashcard` && e.code === `Space`) {
        const tag = (document.activeElement && document.activeElement.tagName) ? document.activeElement.tagName.toLowerCase() : ``;
        if (tag !== `input` && tag !== `button`) {
          e.preventDefault();
          flipFlashcard();
        }
      }
    });

    if (document.readyState === `loading`) {
      document.addEventListener(`DOMContentLoaded`, initApp);
    } else {
      initApp();
    }
  </script>
</body>
</html>
