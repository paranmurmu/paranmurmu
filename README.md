<svg xmlns="http://www.w3.org/2000/svg"
     viewBox="0 0 1180 610"
     width="100%"
     role="img"
     aria-labelledby="title desc">

  <title id="title">Paran Murmu — Developer Profile</title>
  <desc id="desc">Animated cyber glassmorphism GitHub profile banner.</desc>

  <defs>

    <!-- BACKGROUND -->
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop stop-color="#030712"/>
      <stop offset=".5" stop-color="#0F172A"/>
      <stop offset="1" stop-color="#020617"/>
    </linearGradient>

    <!-- MAIN ACCENT -->
    <linearGradient id="accent"
                    x1="0%" y1="0%"
                    x2="100%" y2="0%">
      <stop stop-color="#7C3AED"/>
      <stop offset=".5" stop-color="#22D3EE"/>
      <stop offset="1" stop-color="#10B981">

        <animate
          attributeName="offset"
          values="1;.5;1"
          dur="5s"
          repeatCount="indefinite"/>
      </stop>
    </linearGradient>

    <!-- ASCII GRADIENT -->
    <linearGradient id="ascii"
                    x1="0%" y1="0%"
                    x2="100%" y2="0%">

      <stop stop-color="#7C3AED"/>
      <stop offset=".45" stop-color="#22D3EE"/>
      <stop offset="1" stop-color="#A78BFA">

        <animate
          attributeName="offset"
          values="1;.5;1"
          dur="6s"
          repeatCount="indefinite"/>
      </stop>
    </linearGradient>

    <!-- PURPLE GLOW -->
    <radialGradient id="purpleGlow">
      <stop stop-color="#7C3AED"
            stop-opacity=".25"/>
      <stop offset="1"
            stop-color="#7C3AED"
            stop-opacity="0"/>
    </radialGradient>

    <!-- CYAN GLOW -->
    <radialGradient id="cyanGlow">
      <stop stop-color="#22D3EE"
            stop-opacity=".20"/>
      <stop offset="1"
            stop-color="#22D3EE"
            stop-opacity="0"/>
    </radialGradient>

    <!-- GREEN GLOW -->
    <radialGradient id="greenGlow">
      <stop stop-color="#10B981"
            stop-opacity=".12"/>
      <stop offset="1"
            stop-color="#10B981"
            stop-opacity="0"/>
    </radialGradient>

    <!-- GLOW -->
    <filter id="glow"
            x="-100%"
            y="-100%"
            width="300%"
            height="300%">

      <feGaussianBlur
        stdDeviation="5"
        result="blur"/>

      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>

    </filter>

    <!-- SOFT BLUR -->
    <filter id="blur">
      <feGaussianBlur stdDeviation="35"/>
    </filter>

    <!-- NOISE -->
    <pattern id="noise"
             width="80"
             height="80"
             patternUnits="userSpaceOnUse">

      <circle cx="10" cy="15"
              r=".8"
              fill="#fff"
              opacity=".08"/>

      <circle cx="42" cy="30"
              r=".6"
              fill="#fff"
              opacity=".06"/>

      <circle cx="25" cy="65"
              r=".7"
              fill="#22D3EE"
              opacity=".05"/>

      <circle cx="70" cy="52"
              r=".7"
              fill="#A78BFA"
              opacity=".06"/>
    </pattern>

    <!-- ROUNDED CLIP -->
    <clipPath id="clip">
      <rect width="1180"
            height="610"
            rx="32"/>
    </clipPath>

  </defs>


  <!-- ================================================= -->
  <!-- BACKGROUND -->
  <!-- ================================================= -->

  <g clip-path="url(#clip)">

    <rect width="1180"
          height="610"
          fill="url(#bg)"/>


    <!-- Floating radial gradients -->

    <circle cx="170"
            cy="110"
            r="260"
            fill="url(#purpleGlow)"
            filter="url(#blur)">

      <animateTransform
        attributeName="transform"
        type="translate"
        values="0 0;55 30;0 0"
        dur="14s"
        repeatCount="indefinite"/>

    </circle>


    <circle cx="1030"
            cy="490"
            r="260"
            fill="url(#cyanGlow)"
            filter="url(#blur)">

      <animateTransform
        attributeName="transform"
        type="translate"
        values="0 0;-50 -25;0 0"
        dur="16s"
        repeatCount="indefinite"/>

    </circle>


    <circle cx="650"
            cy="240"
            r="190"
            fill="url(#greenGlow)"
            filter="url(#blur)">

      <animateTransform
        attributeName="transform"
        type="translate"
        values="0 0;25 -30;0 0"
        dur="12s"
        repeatCount="indefinite"/>

    </circle>


    <!-- Noise -->

    <rect width="1180"
          height="610"
          fill="url(#noise)"/>


    <!-- ================================================= -->
    <!-- PARTICLES -->
    <!-- ================================================= -->

    <g fill="#22D3EE"
       filter="url(#glow)">

      <circle cx="80" cy="72" r="1.5">
        <animate
          attributeName="opacity"
          values=".1;1;.1"
          dur="3s"
          repeatCount="indefinite"/>
      </circle>

      <circle cx="480" cy="80" r="1">
        <animate
          attributeName="opacity"
          values="1;.1;1"
          dur="4s"
          repeatCount="indefinite"/>
      </circle>

      <circle cx="1090" cy="120" r="1.3">
        <animate
          attributeName="opacity"
          values=".1;.8;.1"
          dur="2.7s"
          repeatCount="indefinite"/>
      </circle>

      <circle cx="720" cy="550" r="1">
        <animate
          attributeName="opacity"
          values=".8;.1;.8"
          dur="3.5s"
          repeatCount="indefinite"/>
      </circle>

    </g>


    <!-- ================================================= -->
    <!-- LEFT PANEL -->
    <!-- ================================================= -->

    <rect x="32"
          y="32"
          width="420"
          height="546"
          rx="26"
          fill="#0F172A"
          fill-opacity=".68"
          stroke="#FFFFFF"
          stroke-opacity=".09"/>


    <!-- Panel top accent -->

    <rect x="55"
          y="55"
          width="370"
          height="1"
          fill="url(#accent)">

      <animate
        attributeName="opacity"
        values=".3;1;.3"
        dur="3s"
        repeatCount="indefinite"/>

    </rect>


    <text x="62"
          y="82"
          fill="#64748B"
          font-family="monospace"
          font-size="11"
          letter-spacing="2">
      PARAN://PROFILE
    </text>


    <!-- ================================================= -->
    <!-- ASCII PORTRAIT -->
    <!-- ================================================= -->

    <g transform="translate(55 112)"
       font-family="monospace"
       font-size="13"
       font-weight="700"
       fill="url(#ascii)"
       filter="url(#glow)">

      <text y="0">
        ░░░░░░░░░░::::::::::░░░░░░░░░
      </text>

      <text y="17">
        ░░░░░░+################+░░░░
      </text>

      <text y="34">
        ░░░░######################░░░
      </text>

      <text y="51">
        ░░##########################░
      </text>

      <text y="68">
        ░######+..........+######░
      </text>

      <text y="85">
        #####+....-======-....+#####
      </text>

      <text y="102">
        ####+...##############...+####
      </text>

      <text y="119">
        ####+..######....######..+####
      </text>

      <text y="136">
        ####+..######....######..+####
      </text>

      <text y="153">
        ####+..######....######..+####
      </text>

      <text y="170">
        #####+...##############...+####
      </text>

      <text y="187">
        ######+.....########.....+######
      </text>

      <text y="204">
        .######..............######.
      </text>

      <text y="221">
        ..########################..
      </text>

      <text y="238">
        ....####################....
      </text>

      <text y="255">
        ......################......
      </text>

      <text y="272">
        .......######....######.......
      </text>

      <text y="289">
        .....######........######.....
      </text>

      <text y="306">
        ...######............######...
      </text>

      <text y="323">
        .######................######.
      </text>

      <!-- Line-by-line reveal -->

      <animate
        attributeName="opacity"
        values="0;1"
        dur="2.5s"
        fill="freeze"/>

    </g>


    <!-- SCANLINE -->

    <rect x="50"
          y="105"
          width="380"
          height="3"
          fill="url(#accent)"
          opacity=".35">

      <animate
        attributeName="y"
        values="105;485;105"
        dur="4.5s"
        repeatCount="indefinite"/>

    </rect>


    <!-- ASCII FLOAT -->

    <animateTransform
      attributeName="transform"
      type="translate"
      values="0 0;0 -5;0 0"
      dur="5s"
      repeatCount="indefinite"/>


    <text x="62"
          y="515"
          fill="#94A3B8"
          font-family="monospace"
          font-size="12">

      SYSTEM STATUS

      <tspan fill="#10B981">
        ● ONLINE
      </tspan>

    </text>


    <text x="62"
          y="540"
          fill="#64748B"
          font-family="monospace"
          font-size="11">

      creative mind / digital builder

    </text>


    <!-- ================================================= -->
    <!-- RIGHT TERMINAL -->
    <!-- ================================================= -->

    <rect x="476"
          y="32"
          width="672"
          height="546"
          rx="26"
          fill="#0F172A"
          fill-opacity=".78"
          stroke="#FFFFFF"
          stroke-opacity=".09"/>


    <!-- TERMINAL HEADER -->

    <rect x="476"
          y="32"
          width="672"
          height="60"
          rx="26"
          fill="#111827"
          fill-opacity=".65"/>


    <circle cx="506"
            cy="62"
            r="5"
            fill="#EF4444"/>

    <circle cx="524"
            cy="62"
            r="5"
            fill="#F59E0B"/>

    <circle cx="542"
            cy="62"
            r="5"
            fill="#10B981"/>


    <text x="570"
          y="67"
          fill="#64748B"
          font-family="monospace"
          font-size="11">

      paran@github ~ /profile

    </text>


    <!-- AVAILABLE -->

    <rect x="1010"
          y="48"
          width="112"
          height="28"
          rx="14"
          fill="#10B981"
          fill-opacity=".08"
          stroke="#10B981"
          stroke-opacity=".25"/>


    <circle cx="1028"
            cy="62"
            r="4"
            fill="#10B981">

      <animate
        attributeName="opacity"
        values=".3;1;.3"
        dur="2s"
        repeatCount="indefinite"/>

    </circle>


    <text x="1040"
          y="66"
          fill="#6EE7B7"
          font-family="monospace"
          font-size="9">

      AVAILABLE

    </text>


    <!-- ================================================= -->
    <!-- INTRO -->
    <!-- ================================================= -->

    <text x="514"
          y="135"
          fill="#94A3B8"
          font-family="Arial, sans-serif"
          font-size="15">

      Hi 👋

    </text>


    <text x="514"
          y="177"
          fill="#F8FAFC"
          font-family="Arial, sans-serif"
          font-size="34"
          font-weight="800">

      I'm Paran Murmu

    </text>


    <!-- TYPING TEXT -->

    <text x="514"
          y="213"
          fill="url(#accent)"
          font-family="monospace"
          font-size="16"
          font-weight="700">

      Frontend Engineer

      <animate
        attributeName="opacity"
        values="1;1;0;0;1"
        dur="8s"
        repeatCount="indefinite"/>

    </text>


    <!-- CURSOR -->

    <rect x="708"
          y="197"
          width="2"
          height="20"
          fill="#22D3EE">

      <animate
        attributeName="opacity"
        values="1;0;1"
        dur="1s"
        repeatCount="indefinite"/>

    </rect>


    <!-- ================================================= -->
    <!-- PROFILE INFORMATION -->
    <!-- ================================================= -->

    <g font-family="Arial, sans-serif"
       font-size="13"
       fill="#94A3B8">

      <text x="514" y="255">
        ⌖
        <tspan fill="#CBD5E1"> Location</tspan>
        <tspan dx="15">West Bengal, India</tspan>

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1s"
          dur=".7s"
          fill="freeze"/>
      </text>


      <text x="514" y="285">
        ◈
        <tspan fill="#CBD5E1"> Education</tspan>
        <tspan dx="10">Student &amp; Self Learner</tspan>

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1.4s"
          dur=".7s"
          fill="freeze"/>
      </text>


      <text x="514" y="315">
        ⌁
        <tspan fill="#CBD5E1"> Current Focus</tspan>
        <tspan dx="10">Web • AI • Creative Tech</tspan>

        <animate
          attributeName="opacity"
          values="0;1"
          begin="1.8s"
          dur=".7s"
          fill="freeze"/>
      </text>


      <text x="514" y="345">
        ↗
        <tspan fill="#CBD5E1"> Portfolio</tspan>
        <tspan dx="15"
               fill="#22D3EE">
          paran-murmu.dev
        </tspan>

        <animate
          attributeName="opacity"
          values="0;1"
          begin="2.2s"
          dur=".7s"
          fill="freeze"/>
      </text>


      <text x="514" y="375">
        ✉
        <tspan fill="#CBD5E1"> Email</tspan>
        <tspan dx="20">
          hello@paranmurmu.dev
        </tspan>

        <animate
          attributeName="opacity"
          values="0;1"
          begin="2.6s"
          dur=".7s"
          fill="freeze"/>
      </text>

    </g>


    <!-- ================================================= -->
    <!-- SKILLS -->
    <!-- ================================================= -->

    <text x="514"
          y="408"
          fill="#64748B"
          font-family="monospace"
          font-size="11"
          letter-spacing="2">

      SKILLS

    </text>


    <!-- SKILL PILLS -->

    <g font-family="monospace"
       font-size="11"
       font-weight="700">

      <!-- React -->

      <rect x="514" y="420"
            width="70"
            height="29"
            rx="15"
            fill="#22D3EE"
            fill-opacity=".06"
            stroke="#22D3EE"
            stroke-opacity=".35">

        <animateTransform
          attributeName="transform"
          type="scale"
          values="1;1.04;1"
          dur="3s"
          repeatCount="indefinite"/>

      </rect>

      <text x="530"
            y="439"
            fill="#CBD5E1">
        React
      </text>


      <!-- Next -->

      <rect x="592" y="420"
            width="76"
            height="29"
            rx="15"
            fill="#7C3AED"
            fill-opacity=".07"
            stroke="#A78BFA"
            stroke-opacity=".35"/>

      <text x="606"
            y="439"
            fill="#CBD5E1">
        Next.js
      </text>


      <!-- Node -->

      <rect x="676" y="420"
            width="76"
            height="29"
            rx="15"
            fill="#10B981"
            fill-opacity=".07"
            stroke="#10B981"
            stroke-opacity=".35"/>

      <text x="690"
            y="439"
            fill="#CBD5E1">
        Node.js
      </text>


      <!-- TypeScript -->

      <rect x="760" y="420"
            width="96"
            height="29"
            rx="15"
            fill="#22D3EE"
            fill-opacity=".06"
            stroke="#22D3EE"
            stroke-opacity=".35"/>

      <text x="775"
            y="439"
            fill="#CBD5E1">
        TypeScript
      </text>


      <!-- Tailwind -->

      <rect x="864" y="420"
            width="88"
            height="29"
            rx="15"
            fill="#22D3EE"
            fill-opacity=".06"
            stroke="#22D3EE"
            stroke-opacity=".35"/>

      <text x="879"
            y="439"
            fill="#CBD5E1">
        Tailwind
      </text>


      <!-- Python -->

      <rect x="960" y="420"
            width="70"
            height="29"
            rx="15"
            fill="#7C3AED"
            fill-opacity=".06"
            stroke="#A78BFA"
            stroke-opacity=".35"/>

      <text x="976"
            y="439"
            fill="#CBD5E1">
        Python
      </text>


      <!-- Docker -->

      <rect x="1038" y="420"
            width="70"
            height="29"
            rx="15"
            fill="#22D3EE"
            fill-opacity=".06"
            stroke="#22D3EE"
            stroke-opacity=".35"/>

      <text x="1052"
            y="439"
            fill="#CBD5E1">
        Docker
      </text>


      <!-- Row 2 -->

      <rect x="514" y="458"
            width="72"
            height="29"
            rx="15"
            fill="#7C3AED"
            fill-opacity=".06"
            stroke="#A78BFA"
            stroke-opacity=".35"/>

      <text x="527"
            y="477"
            fill="#CBD5E1">
        Postgres
      </text>


      <rect x="594" y="458"
            width="76"
            height="29"
            rx="15"
            fill="#10B981"
            fill-opacity=".06"
            stroke="#10B981"
            stroke-opacity=".35"/>

      <text x="608"
            y="477"
            fill="#CBD5E1">
        AWS
      </text>


      <rect x="678" y="458"
            width="56"
            height="29"
            rx="15"
            fill="#22D3EE"
            fill-opacity=".06"
            stroke="#22D3EE"
            stroke-opacity=".35"/>

      <text x="693"
            y="477"
            fill="#CBD5E1">
        Git
      </text>


      <rect x="742" y="458"
            width="70"
            height="29"
            rx="15"
            fill="#7C3AED"
            fill-opacity=".06"
            stroke="#A78BFA"
            stroke-opacity=".35"/>

      <text x="756"
            y="477"
            fill="#CBD5E1">
        Figma
      </text>

    </g>


    <!-- ================================================= -->
    <!-- SOCIAL -->
    <!-- ================================================= -->

    <g font-family="monospace"
       font-size="12"
       fill="#94A3B8">

      <text x="514" y="530">
        GitHub
      </text>

      <text x="595" y="530">
        LinkedIn
      </text>

      <text x="690" y="530">
        Twitter
      </text>

      <text x="775" y="530">
        Portfolio
      </text>

    </g>


    <!-- SOCIAL ICONS -->

    <g fill="none"
       stroke="url(#accent)"
       stroke-width="1.6"
       filter="url(#glow)">

      <circle cx="565" cy="526" r="8"/>

      <rect x="660"
            y="518"
            width="15"
            height="15"
            rx="2"/>

      <path d="M745 519L760 526L745 533Z"/>

      <circle cx="850"
              cy="526"
              r="8"/>

    </g>


    <!-- ================================================= -->
    <!-- MOVING SCANLINE -->
    <!-- ================================================= -->

    <rect x="0"
          y="0"
          width="1180"
          height="2"
          fill="url(#accent)"
          opacity=".25">

      <animate
        attributeName="y"
        values="0;610;0"
        dur="7s"
        repeatCount="indefinite"/>

    </rect>


    <!-- ================================================= -->
    <!-- BORDER SHIMMER -->
    <!-- ================================================= -->

    <rect x="1"
          y="1"
          width="1178"
          height="608"
          rx="32"
          fill="none"
          stroke="url(#accent)"
          stroke-width="1.5"
          stroke-opacity=".65">

      <animate
        attributeName="stroke-opacity"
        values=".25;.8;.25"
        dur="4s"
        repeatCount="indefinite"/>

    </rect>

  </g>

</svg>
