# Different Ways to Jump Bug as of 28/02/2025

## Comparison

| Method                                      | Works on Any Height | Easier Timing | Does not require Special Binds | Isn't Cheeto |
|----------------------------------------------|---------------------|---------------|------------------------|-------------------|
| **Manual JB**                                | ✅                  | ❌            | ✅                     | ✅                |
| **Desubticked JB Radio Bind**                | ❌                  | ✅            | ❌                     | ✅                |
| **Subticked JB Wooting DKS Bind**            | ✅                  | ❌            | ❌                     | ❌                |
| **Subticked JB Macro Bind**                  | ✅                  | ❌            | ❌                     | ❌                |
| **Desubticked JB `sv_cheats 1` Async Exploit** | ❌               | ✅            | ❌                     | ❌                |

---

## Methods:

### 1. **Manual JB**

- **Description:** Use regular binds like `+duck` and `+jump`. Start scrolling your mouse wheel before landing and simply unduck.  
- **Pros:**  
  - Works on any height  
  - No special configurations needed  
- **Cons:**  
  - Requires precise timing for unduck and jump in the same subtick  
  - Timing varies based on height and tick alignment  

---


### 2. **Desubticked JB Radio Bind**

- **Description:** Uses radial binds for multibind support. Once in optimal JB height press and release your KEY bind (bind will execute once you let go of the key). 
- **Configuration:**

autoexec.cfg
```
bind KEY +radialradio1 //replace KEY with your desired key like mouse5
cl_radialmenu_deadzone_size 0
cl_radial_radio_tab_1_text_1 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_2 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_3 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_4 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_5 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_6 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_7 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
cl_radial_radio_tab_1_text_8 cmd";duck -999 0 0; jump 1 0 0; jump -999 0 0;
```
  
- **Pros:**  
  - Easier timing with +/-16ms buffer  
  - Engine-level multibind
- **Cons:**  
  - Unusual bind, requires practice  
  - Restricted to 64-tick heights
  - Cant look around while bind is pressed in

---

### 3. **Subticked JB Wooting DKS Bind**

- **Description:** Set up a Wooting DKS bind to press duck on the way in and press jump on the way up. Use KEY to duck and once in optimal JB height simply release KEY.
- **Configuration:**
autoexec.cfg
```
bind KEY "+duck" //replace KEY with your desired key like "alt"
```
![image](https://github.com/user-attachments/assets/c57b314f-008a-4e0a-a191-2682a6245386)

- **Pros:**  
  - Works on any height  
- **Cons:**  
  - Timing varies based on height  
  - Considered cheeto 
  - Requires Wooting Keyboard

---

### 4. **Subticked JB Macro Bind**

- **Description:** Set up macros to press unduck and jump simultaneously. Once in optimal JB height press your macro key.
- **Configuration:**
autoexec.cfg
```
bind KEY1 "duck -999 0 0" //replace KEY1 with your desired key like "o"
bind KEY2 "+jump" //replace KEY2 with your desired key like "i"
```

- **Pros:**  
  - Works on any height  
- **Cons:**  
  - Timing varies based on height  
  - Considered cheeto 

---


### 6. **Desubticked JB Async Exploit (`sv_cheats 1`)**

- **Description:** Uses an exploit to bypass `sv_cheats 1` and asynchronously execute a COD4 like sleep cfg (flashbacks :aware:).  
- **Reference:** [Steam Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=3313210014)  
- **Pros:**  
  - Easier timing and multibind support  
- **Cons:**  
  - Requires to make use of exec_async which is usually locked behind `sv_cheats 1` unless executed from the lobby
  - Considered cheeto and can be misused to various other movement automation shenanigans like autohop or a movement recorder
  - Restricted to 64-tick heights
  - Needs manual reexecution after a certain amount of time
  - Input consistency is FPS related

---

> [!NOTE]  
> "Restricted to 64-tick heights" can be worked around by using a LJ bind to manipulate the takeoff height and therefore make the tick align the optimal JB bind height
