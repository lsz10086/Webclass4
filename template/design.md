* # Design System

  Dark coral SaaS style — derived from template/topheader.jpg & template/howitworks.jpg.
  Use this document as the single source of truth for all new pages in this project.

  ## 1. Color

  | Token                   | Hex / Value                 | Usage                                              |
  | :---------------------- | :-------------------------- | :------------------------------------------------- |
  | `--primary`             | `#f04d66`                   | Brand accent, primary CTA, step badges, highlights |
  | `--primary-hover`       | `#ff6379`                   | Primary button / link hover                        |
  | `--primary-soft`        | `rgba(240, 77, 102, 0.16)`  | Soft tag / chip background                         |
  | `--secondary-btn`       | `#3d4b46`                   | Secondary button fill                              |
  | `--secondary-btn-hover` | `#4a5a54`                   | Secondary button hover                             |
  | `--page-background`     | `#0a1210`                   | Page background (App background)                   |
  | `--card-background`     | `#121c1a`                   | Card default background                            |
  | `--text-primary`        | `#f4f7f6`                   | Main headings, primary text                        |
  | `--text-muted`          | `#8b9793`                   | Paragraphs, descriptions, secondary text           |
  | `--border-default`      | `rgba(255, 255, 255, 0.06)` | Default borders for cards and containers           |
  | `--border-hover`        | `rgba(240, 77, 102, 0.28)`  | Card border on hover state                         |

  ## 2. Typography

  *   **Font Family**: `Inter`, "Segoe UI", sans-serif
  *   **H1 (Main Title)**: `2.15rem`, weight `700`, line-height `1.2`, letter-spacing `-0.03em`
  *   **H2 (Section Title)**: `1.35rem`, weight `650`, letter-spacing `-0.02em`
  *   **H3 (Card Title)**: `0.88rem`, weight `600`, line-height `1.55`
  *   **Body / Description**: `0.92rem` (Hero p), `0.75rem` (Card desc), weight `400`
  *   **Tag / Chip**: `0.72rem`, weight `500`

  ## 3. Spacing & Layout

  *   **Container Max Width**: `880px` (Centered)
  *   **Page Padding**: `2.4rem 1.2rem 3.2rem` (Top, Left/Right, Bottom)
  *   **Grid Gap**: `0.7rem`
  *   **Hero Margin Bottom**: `2.8rem`
  *   **Section Title Margin Bottom**: `1.25rem`
  *   **Card Inner Padding**: `0.65rem` to `0.75rem`

  ## 4. Components

  ### Cards (Meal / Work Item)
  *   **Radius**: `20px` (`--radius-card`)
  *   **Shadow**: `0 8px 24px rgba(0, 0, 0, 0.22)`
  *   **Transition**: `0.22s ease` (transform, background, border-color)
  *   **Hover State**:
      *   Transform: `translateY(-3px)`
      *   Background: `var(--card-hover)` (`#162220`)
      *   Border Color: `var(--border-hover)` (`rgba(240, 77, 102, 0.28)`)

  ### Image Preview (Inside Card)
  *   **Radius**: `12px`
  *   **Border**: `1px solid var(--border-default)`
  *   **Height**: `96px` (Desktop), `140px` (Mobile <= 560px)
  *   **Object Fit**: `cover`

  ### Tags / Chips (Category)
  *   **Radius**: `999px` (Pill shape)
  *   **Padding**: `2px 8px`
  *   **Background**: `var(--primary-soft)`
  *   **Text Color**: `var(--primary)`

  ### Step Badges (Number Circle)
  *   **Size**: `16px * 16px`
  *   **Radius**: `50%`
  *   **Background**: `var(--primary)`
  *   **Text Color**: `#ffffff`

  ## 5. CSS Variable Reference (`:root`)

  ```css
  :root {
    /* Colors */
    --primary: #f04d66;
    --primary-hover: #ff6379;
    --primary-soft: rgba(240, 77, 102, 0.16);
    --secondary-btn: #3d4b46;
    --secondary-btn-hover: #4a5a54;
    
    --bg: #0a1210;
    --card: #121c1a;
    --card-hover: #162220;
    
    --text: #f4f7f6;
    --text-muted: #8b9793;
    
    --border-default: rgba(255, 255, 255, 0.06);
    --border-hover: rgba(240, 77, 102, 0.28);
  
    /* Borders & Shadows */
    --radius-card: 20px;
    --radius-pill: 999px;
    --shadow: 0 8px 24px rgba(0, 0, 0, 0.22);
    --transition: 0.22s ease;
  }