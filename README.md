# Longevity Age Estimator — PWA

Εκτίμηση βιολογικής ηλικίας με PhenoAge algorithm (Levine et al. 2018).

## Εγκατάσταση στο κινητό (GitHub Pages)

### Βήμα 1 — Δημιούργησε repository στο GitHub
1. Πήγαινε στο github.com → New repository
2. Όνομα: `longevity-app` (ή ό,τι θες)
3. Public ✓ → Create repository

### Βήμα 2 — Upload τα αρχεία
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/USERNAME/longevity-app.git
git push -u origin main
```

### Βήμα 3 — Ενεργοποίησε GitHub Pages
1. Repository → Settings → Pages
2. Source: Deploy from a branch → main / root
3. Save

Σε ~2 λεπτά το app είναι live στο:
`https://USERNAME.github.io/longevity-app`

### Βήμα 4 — Εγκατάσταση στο Android
1. Άνοιξε το URL σε **Chrome**
2. Πάτα το μενού (3 τελείες) → **"Προσθήκη στην αρχική οθόνη"**
3. Επιβεβαίωσε → Εγκατεστημένο! 🎉

Λειτουργεί και **offline** (service worker cache).

## Αρχεία
- `index.html` — Το κύριο app
- `manifest.json` — PWA metadata
- `sw.js` — Service worker (offline support)
- `icons/` — App icons

## Algorithm
Βασισμένο στο **PhenoAge** (Morgan Levine, Yale 2018).
Χρησιμοποιεί: WBC, κρεατινίνη, MCV, αιμοπετάλια, αιμοσφαιρίνη,
βιταμίνη D3, B12, λιπιδαιμικό προφίλ, τριγλυκερίδια.
