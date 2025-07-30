# 🛒 Redux Cart Demo  

A practice project implementing **Redux Toolkit (RTK)** for a scalable e-commerce cart system with:  
- ✅ User authentication (login/logout)  
- 🛍️ Cart operations (add/remove/update items)  
- 🔄 State persistence (optional)  

## **Tech Stack**  
- React 18  
- Redux Toolkit (RTK)  
- React Router v6  
- CSS Modules 

## **Features**  
### **1. Redux-Powered Cart**  
- Add/remove items with quantity controls  
- Dynamic total calculation  
- Cart visibility toggle  

### **2. User Authentication**  
- Mock login/logout flow  
- Protected routes (e.g., `/cart` only for logged-in users)  

### **3. Clean State Management**  
```javascript
// Example slice (cartSlice.js)  
const cartSlice = createSlice({
  name: 'cart',
  initialState: { items: [], isVisible: false },
  reducers: {
    addItem: (state, action) => {
      state.items.push(action.payload); 
    },
    // ... other reducers
  },
});
