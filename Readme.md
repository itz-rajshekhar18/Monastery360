## 📂 Project Structure

```text
monastery360-mvp/
├── backend/
│   ├── .env
│   ├── .env.example
│   ├── .gitignore
│   ├── requirements.txt
│   ├── README.md
│   ├── alembic.ini
│   ├── alembic/
│   │   ├── versions/
│   │   ├── env.py
│   │   ├── script.py.mako
│   │   └── README
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py
│   │   ├── core/
│   │   │   ├── __init__.py
│   │   │   ├── config.py
│   │   │   ├── security.py
│   │   │   └── database.py
│   │   ├── api/
│   │   │   ├── __init__.py
│   │   │   └── v1/
│   │   │       ├── __init__.py
│   │   │       ├── router.py
│   │   │       └── endpoints/
│   │   │           ├── __init__.py
│   │   │           ├── auth.py
│   │   │           ├── monasteries.py
│   │   │           ├── tours.py
│   │   │           ├── media.py
│   │   │           └── maps.py
│   │   ├── models/
│   │   │   ├── __init__.py
│   │   │   ├── base.py
│   │   │   ├── user.py
│   │   │   ├── monastery.py
│   │   │   ├── tour.py
│   │   │   └── media.py
│   │   ├── schemas/
│   │   │   ├── __init__.py
│   │   │   ├── user.py
│   │   │   ├── monastery.py
│   │   │   ├── tour.py
│   │   │   └── media.py
│   │   ├── services/
│   │   │   ├── __init__.py
│   │   │   ├── auth_service.py
│   │   │   ├── monastery_service.py
│   │   │   ├── tour_service.py
│   │   │   ├── media_service.py
│   │   │   └── s3_service.py
│   │   └── utils/
│   │       ├── __init__.py
│   │       ├── dependencies.py
│   │       ├── exceptions.py
│   │       └── helpers.py
│   └── tests/
│       ├── __init__.py
│       ├── conftest.py
│       ├── test_auth.py
│       ├── test_monasteries.py
│       └── test_tours.py
└── frontend/
    ├── .env.local
    ├── .env.example
    ├── .gitignore
    ├── package.json
    ├── next.config.js
    ├── tailwind.config.js
    ├── tsconfig.json
    ├── README.md
    ├── public/
    │   ├── images/
    │   ├── icons/
    │   └── favicon.ico
    ├── src/
    │   ├── app/
    │   │   ├── layout.tsx
    │   │   ├── page.tsx
    │   │   ├── globals.css
    │   │   ├── loading.tsx
    │   │   ├── error.tsx
    │   │   ├── not-found.tsx
    │   │   ├── auth/
    │   │   │   ├── login/
    │   │   │   │   └── page.tsx
    │   │   │   └── register/
    │   │   │       └── page.tsx
    │   │   ├── monasteries/
    │   │   │   ├── page.tsx
    │   │   │   ├── [id]/
    │   │   │   │   └── page.tsx
    │   │   │   └── components/
    │   │   │       ├── MonasteryCard.tsx
    │   │   │       ├── MonasteryList.tsx
    │   │   │       └── MonasteryDetail.tsx
    │   │   ├── tours/
    │   │   │   ├── page.tsx
    │   │   │   ├── [id]/
    │   │   │   │   └── page.tsx
    │   │   │   └── components/
    │   │   │       ├── Tour360Viewer.tsx
    │   │   │       ├── TourList.tsx
    │   │   │       └── TourNavigation.tsx
    │   │   ├── maps/
    │   │   │   ├── page.tsx
    │   │   │   └── components/
    │   │   │       ├── InteractiveMap.tsx
    │   │   │       └── MonasteryMarker.tsx
    │   │   └── dashboard/
    │   │       ├── page.tsx
    │   │       └── layout.tsx
    │   ├── components/
    │   │   ├── ui/
    │   │   │   ├── button.tsx
    │   │   │   ├── card.tsx
    │   │   │   ├── input.tsx
    │   │   │   ├── modal.tsx
    │   │   │   └── loading-spinner.tsx
    │   │   ├── layout/
    │   │   │   ├── Header.tsx
    │   │   │   ├── Footer.tsx
    │   │   │   ├── Sidebar.tsx
    │   │   │   └── Navigation.tsx
    │   │   ├── forms/
    │   │   │   ├── LoginForm.tsx
    │   │   │   ├── RegisterForm.tsx
    │   │   │   └── ContactForm.tsx
    │   │   └── media/
    │   │       ├── Image360Viewer.tsx
    │   │       ├── VideoPlayer.tsx
    │   │       └── MediaGallery.tsx
    │   ├── lib/
    │   │   ├── api.ts
    │   │   ├── auth.ts
    │   │   ├── utils.ts
    │   │   ├── constants.ts
    │   │   └── validations.ts
    │   ├── hooks/
    │   │   ├── useAuth.ts
    │   │   ├── useMonasteries.ts
    │   │   ├── useTours.ts
    │   │   └── useGeolocation.ts
    │   ├── context/
    │   │   ├── AuthContext.tsx
    │   │   ├── ThemeContext.tsx
    │   │   └── AppContext.tsx
    │   ├── types/
    │   │   ├── auth.ts
    │   │   ├── monastery.ts
    │   │   ├── tour.ts
    │   │   └── api.ts
    │   └── styles/
    │       ├── globals.css
    │       └── components.css
    └── docs/
        ├── API.md
        └── SETUP.md
