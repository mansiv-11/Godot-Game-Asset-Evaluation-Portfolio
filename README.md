
# Godot / Game Asset Evaluation Portfolio  
By Mansi Verma – AI Evaluation Fellow (Project Helix)  

This portfolio showcases my process for evaluating Godot scenes and digital game assets for AI and research workflows.  
I focus on clear documentation, guideline-based reviews, and attention to detail.

---

## 1. Scene Structure Evaluation

These samples show how I review Godot scene hierarchies:

- Check node naming consistency  
- Verify parent–child relationships  
- Identify missing or redundant nodes  
- Note any hierarchy changes needed for clarity or reuse  

Example findings (from sample files in `scene-evaluations/`):

- Root node is correctly set to `Node2D`, but UI nodes should be grouped under a separate `CanvasLayer`.  
- CollisionShape2D nodes exist, but names like `CollisionShape2D2` should be renamed to describe their purpose (e.g., `PlayerHitbox`).  

---

## 2. Asset Quality & Visual Consistency

I review 2D assets (sprites, tiles, UI) for:

- Resolution and pixel consistency  
- Blurriness or stretching  
- Color palette mismatches  
- Transparency / background issues  

Example findings (see `asset-quality-reviews/`):

- Several sprites were exported at different resolutions, leading to visible size jumps.  
- One tileset had a faint white outline around tiles due to incorrect export settings; recommended re-export with proper alpha.  

---

## 3. Animation Consistency Checks

For animations, I focus on:

- Frame timing and smoothness  
- Loop quality  
- Pose and motion consistency  
- Start / end pose alignment  

Example notes (see `animation-checks/`):

- Walk cycle is smooth, but the idle animation pops because the first frame and last frame do not match.  
- Attack animation has good anticipation but needs an extra recovery frame to feel natural.  

---

## 4. Physics & Collision Review

Here I verify:

- Collision shapes match visible sprites  
- Hitboxes do not extend far outside visuals  
- Objects use appropriate layers and masks  
- Basic gravity and movement feel correct in playtests  

Example notes (see `physics-collision/`):

- Player hitbox is slightly taller than the sprite and causes early ground contact on slopes.  
- Enemy collision shape overlaps the environment; suggested separate hurtbox and body shape.  

---

## 5. Guideline-Based Evaluation

Many of my tasks involve reading detailed guidelines and applying them consistently.  
Sample reports in `guideline-based-reviews/` show:

- Checklist-style scoring (pass / fail per rule)  
- Short, clear comments for each violation  
- Final summary explaining impact and priority  

---

## 6. Related Background

**AI Evaluation Fellow – Project Helix (Handshake AI)**  
- Review complex pull requests and technical tasks for difficulty, validity, and clarity  
- Follow multi-step guidelines and provide structured, written feedback  
- Work with model-generated assets and edge cases  

**M.S. in Data Science – Western Michigan University**  
- Machine learning, model evaluation, and data quality  
- Strong analytical and documentation skills  

---

## 7. Contact

Email: mansi.verma5858@gmail.com  
GitHub: https://github.com/mansiv-11  
LinkedIn: https://www.linkedin.com/in/mansi-verma-07a9071b3/
