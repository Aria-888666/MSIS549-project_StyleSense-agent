## System Architecture

### Overview

StyleSense uses a hybrid architecture combining:
- Context processing
- Rule-based validation
- Generative AI
- Cloud image processing

---

### Components

#### 1. Frontend (Lovable)

- Context input page
- Dressing room interface
- Outfit display
- Virtual try-on upload
- Animated transitions (Framer Motion)

---

#### 2. Context Agent

Processes:
- Weather
- Occasion
- Gender
- Natural language preferences

Extracts keywords such as:
- "no jeans"
- "no pants"
- "not rain"
- Style preferences

Outputs structured constraints.

---

#### 3. Constraint Engine

Applies rule-based validation:

- Bottom required if top selected (unless dress)
- Shoes always required
- Only selected wardrobe items allowed
- Remove items based on negative keywords
- Provide alternative items if missing

---

#### 4. Styling Agent (OpenAI)

Input:
- Context
- Selected items
- Constraints

Output:
- Three independent outfit combinations
- Style explanations
- Color coordination
- Purchase suggestions

---

#### 5. Backend (Supabase)

- Edge Functions for virtual try-on
- Image processing
- Error handling for function responses

---

### Workflow

1. User enters context  
2. Context agent extracts constraints  
3. Wardrobe filtered dynamically  
4. User selects items  
5. OpenAI generates outfits  
6. Constraint engine validates outputs  
7. Results displayed  
8. Optional virtual try-on  

---

### Key Design Decisions

- Hybrid AI + rule-based approach for reliability  
- Independent generation for diversity  
- Dynamic wardrobe filtering before generation  
