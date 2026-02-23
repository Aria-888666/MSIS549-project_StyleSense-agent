## StyleSense – AI Outfit Decision Agent

Live App:
https://stylesense-outfits-deisgn.lovable.app

Demo Video:
[https://drive.google.com/file/d/1Pya_V7tLNvYt0KPdwriHKg8fMLBJRGbn/view?usp=sharing]

---

### Overview

StyleSense is an AI-powered personal styling assistant that helps users decide what to wear based on daily context such as weather, occasion, and personal preferences.

The system generates multiple outfit recommendations, allows users to virtually try on outfits, and provides shopping suggestions at different price levels.

This project was built for MSIS 549: AI and GenAI for Business Applications.

---

### Problem

Choosing daily outfits requires balancing multiple factors:
- Weather
- Occasion
- Comfort
- Personal style
- Available wardrobe

This often leads to:
- Decision fatigue
- Wasted time
- Underused clothing
- Inefficient purchases

---

### Solution

StyleSense provides a context-aware AI agent that:

1. Collects daily context and preferences  
2. Filters wardrobe options dynamically  
3. Generates three independent outfit recommendations  
4. Explains reasoning for each outfit  
5. Allows virtual try-on using uploaded photos  
6. Suggests purchase options with price levels  

---

### Key Features

- Natural language preference input (e.g., "no jeans", "formal but comfortable")
- Dynamic wardrobe filtering based on context
- Three independent outfit options
- Constraint validation (required items, selected items only)
- Virtual try-on using Supabase Edge Functions
- Shopping suggestions (low / medium / high price)
- Cinematic “magical dressing room” experience

---

### Tech Stack

Frontend:
- Lovable
- Framer Motion

AI:
- OpenAI API

Backend:
- Supabase
- Edge Functions

---

### How to Reproduce

1. Open the live application  
2. Enter context (weather, occasion, preferences)  
3. Select wardrobe items  
4. Generate outfit recommendations  
5. (Optional) Upload photo for virtual try-on  

---

### Future Improvements

- Persistent user profiles
- Real retailer API integration
- Improved virtual fitting accuracy
- Mobile application
