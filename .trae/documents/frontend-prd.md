## 1. Product Overview
Intelligent Crop Yield Prediction & Agentic Farm Advisory System (Frontend Redesign)
- **Purpose**: To provide a production-grade, highly aesthetic UI (10/10 visual quality) for predicting crop yields and receiving agentic agronomy advice. 
- **Target Users**: Farmers, Agronomists, and Agricultural Researchers.
- **Value**: Transforms a standard ML project into a premium SaaS-like experience with beautiful glassmorphism effects, smooth page transitions, and interactive animated charts.

## 2. Core Features

### 2.1 Feature Module
1. **Landing/Home Page**: Modern hero section with glassmorphism, value proposition, and call-to-action.
2. **Dashboard / Data Explorer**: Interactive Recharts/Chart.js animated charts showing feature correlations and historical yield distributions.
3. **Prediction Interface**: Sleek input forms with floating labels and instant feedback for yield prediction.
4. **Agentic Advisory Interface**: A chat-like or Notion-like structured view for the LangGraph agent's agronomy report, complete with a skeleton loading state.

### 2.2 Page Details
| Page Name | Module Name | Feature description |
|-----------|-------------|---------------------|
| Home | Hero Section | Premium glassmorphism card, bold typography, call-to-action to "Start Predicting". |
| Data Explorer | Analytics View | Animated charts (Recharts) displaying historical data trends. Includes a new Drag & Drop zone to upload custom CSV datasets. |
| Predict Yield | Input Form | Sleek, validation-enabled form for weather/soil inputs. Animated result reveal. |
| Advisory Agent | Report View | Notion-like clean layout displaying the AI's structured advice. Skeleton loaders during API calls. |

## 3. Core Process
1. User lands on the modern Home Page and clicks "Start Predicting".
2. User explores historical data trends in the Data Explorer via animated charts.
3. User inputs farm conditions (Rainfall, Temp, Crop Type) into the Predict Yield form.
4. The system communicates with the FastAPI backend and smoothly reveals the predicted yield.
5. User clicks "Generate Advisory Report", triggering a skeleton loading state while the LangGraph agent processes the request.
6. The Agent's structured report is displayed in a highly readable, premium format.

## 4. User Interface Design

### 4.1 Design Style
- **Aesthetic**: Ultra-Premium Dark Mode ONLY. Brutally minimal with extreme glassmorphism. Deep space black (#000000) with highly polished glass panels. Absolutely NO green shadows or glowing colors anywhere. 
- **Typography**: Clash Display or Space Grotesk for dramatic, modern headers. JetBrains Mono for data points and UI text. No generic fonts.
- **Color Palette**: Pure Black (`#000000`) background. UI elements are pure frosted glass (white/10 to white/5) with aggressive background blur (`backdrop-blur-3xl`). ALL shadows must be stark white (`rgba(255,255,255,x)`). No green or neon colors. 
- **UI Elements**: True glassmorphism. Borderless or 1px hairline borders (`border-white/10`). Intense stark white drop shadows behind glass cards on hover. Buttons are stark white, and hover effects use pure white glowing shadows.
- **Motion**: Cinematic and Highly Advanced. Complex staggered reveals, scroll-linked parallax, continuous floating elements, magnetic hover effects on all interactive elements. The home page must feel alive and dynamic, pushing the limits of Framer Motion.


### 4.2 Page Design Overview
| Page Name | Module Name | UI Elements |
|-----------|-------------|-------------|
| Home | Hero | Large typography, glowing gradient or mesh background, primary CTA button. |
| Data Explorer | Charts | Recharts components with tooltips, custom stylized axes, and smooth entry animations. |
| Predict Yield | Form | Floating label inputs, sliders with custom track colors, prominent submit button with loading spinner. |
| Advisory | Report | Markdown rendering area with clean typography, distinct section headers, and a "Download PDF" action button. |

### 4.3 Responsiveness
- Desktop-first design optimized for large analytical dashboards, but fully fluid and mobile-adaptive using Tailwind's responsive utility classes. Touch-friendly inputs for sliders and dropdowns.