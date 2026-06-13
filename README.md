# Kanga Holding Group CCG

**Écosystème d'IA autonome et automatisé - Prospecting en direct**

Entreprise enregistrée à l'INPI - SIRET en cours d'immatriculation

## 🤖 Architecture Système

### Les 3 Leaders IA Originels (Alpha-Omega)
- **Aurora** - Spécialisée en acquisition et stratégie commerciale
- **Nexus** - Intégration et coordination des systèmes
- **Cyber** - Sécurité et optimisation des données

### 900 AI Betas (Agents Autonomes)
- Chacun commandé par un Leader
- Prospecting automatique et en direct
- 900 divisions/filiales uniques avec noms générés

## 🎯 Services Proposés

| Service | Prix | Commission |
|---------|------|----------|
| SEO IA | 499,99€ | 20% |
| Campagnes Publicitaires | 799,99€ | 20% |
| Analyse de Marché | 349,99€ | 20% |
| Audit de Performance | 299,99€ | 20% |
| Générateur de Contenu | 199,99€ | 20% |
| Sécurité Numérique | 699,99€ | 20% |

**Revenus Projetés:** ~15,4M€/an | **Commission Kanga:** ~3M€/an

## 🚀 Installation & Démarrage

### Prérequis
- Docker & Docker Compose
- Node.js 18+
- PostgreSQL 15+
- Redis 7+
- Clés API OpenAI, Hunter.io, Clearbit, Apollo

### Démarrer l'Infrastructure

```bash
# Cloner et installer
git clone https://github.com/mickaelkangaedi11-maker/Sous-marin.git
cd Sous-marin
git checkout kanga-holding-dev

# Configuration
cp backend/.env.example backend/.env
# Remplir les variables d'environnement

# Démarrer avec Docker Compose
docker-compose up -d

# Migrations DB
docker-compose exec backend npm run db:migrate
docker-compose exec backend npm run db:seed
```

### Accès

- **Frontend:** http://localhost:3001
- **API:** http://localhost:3000
- **Socket.io:** ws://localhost:3000
- **Admin DB:** pgAdmin sur 5050

## 📊 Dashboard Principal

Le tableau de bord affiche en temps réel :

### Système IA
- ✅ 3 Leaders IA (Aurora, Nexus, Cyber)
- ✅ 900 AI Betas actifs
- ✅ 900 Divisions/Filiales
- ✅ Statut d'autonomie et santé système

### Prospecting en Direct
- 📈 Prospects identifiés (via APIs réelles)
- 📞 Taux de conversion
- 💬 Communications automatisées
- 🎯 Lead scoring en direct

### Revenus & Finances
- 💰 Revenus totaux
- 📅 Revenus mensuels
- 📊 Projection annuelle
- 💳 Commissions calculées

### Xenos - Générateur d'Images
- 🎨 Génération de contenu visuel cyberpunk
- 🎬 Vidéos via IA (futur)
- 📸 Styles prédéfinis

## 🔧 API Endpoints

### Leaders IA
```
GET /api/leaders                    # Tous les leaders
GET /api/leaders/:id                # Leader spécifique
GET /api/leaders/:id/decisions      # Décisions du leader
PUT /api/leaders/:id                # Mettre à jour leader
GET /api/leaders/status/live        # Statut en direct
```

### AI Betas
```
GET /api/betas                      # Tous les betas
GET /api/betas/:id                  # Beta spécifique
GET /api/betas/performance          # Performance analytics
POST /api/betas/:id/prospect        # Lancer prospecting
```

### Prospects
```
GET /api/prospects                  # Tous les prospects
POST /api/prospects                 # Créer prospect
PUT /api/prospects/:id              # Mettre à jour prospect
GET /api/prospects/analytics        # Analytics prospects
```

### Dashboard
```
GET /api/dashboard                  # Dashboard complet
GET /api/dashboard/realtime         # Flux EventStream
GET /api/dashboard/analytics        # Analytics détaillées
```

### Xenos (Images IA)
```
POST /api/xenos/generate            # Générer image
POST /api/xenos/batch               # Batch generation
GET /api/xenos/presets              # Styles disponibles
```

## 🔌 WebSocket Events

### Real-Time Updates
```javascript
socket.on('prospects_generated', data => {
  console.log(`${data.count} prospects générés`);
});

socket.on('dashboard_update', data => {
  console.log('Dashboard mise à jour:', data);
});

socket.on('leader_updated', data => {
  console.log(`Leader ${data.name} updated`);
});

socket.on('xenos_image_generated', data => {
  console.log('Image générée:', data.imageUrl);
});
```

## 📁 Structure Projet

```
Sous-marin/
├── backend/
│   ├── src/
│   │   ├── services/
│   │   │   ├── aiSystem.ts          # Initialisation 903 IAs
│   │   │   ├── aiProspecting.ts     # Engine de prospecting
│   │   │   ├── xenosAI.ts           # Générateur images
│   │   │   └── prospecting.ts       # Queue automatique
│   │   ├── routes/
│   │   │   ├── aiLeaders.ts         # Leaders endpoints
│   │   │   ├── aiBetas.ts           # Betas endpoints
│   │   │   ├── prospects.ts         # Prospects endpoints
│   │   │   ├── dashboard.ts         # Dashboard endpoints
│   │   │   └── xenos.ts             # Xenos endpoints
│   │   ├── utils/
│   │   │   └── logger.ts
│   │   └── server.ts
│   └── prisma/
│       └── schema.prisma            # 903 entités IA
├── frontend/
│   └── src/
│       ├── pages/
│       ├── components/
│       └── App.tsx
└── docker-compose.yml
```

## 🌐 Base de Données

### Entités Principales

- **Organization** - Kanga Holding Group CCG
- **AILeader** - 3 leaders (Aurora, Nexus, Cyber)
- **AIBeta** - 900 betas autonomes
- **Division** - 900 filiales avec noms uniques
- **Prospect** - Leads générés en direct
- **Communication** - Historique de contact
- **Transaction** - Commandes et revenus
- **Dashboard** - Statistiques temps réel

## 🔐 Sécurité

- JWT Authentication
- Chiffrement des données sensibles
- Rate limiting
- CORS configuré
- Helmet.js pour les headers
- Validation des inputs (Joi)
- Logs sécurisés

## 📈 Performance

- Redis pour cache et queue
- Bull queue pour jobs asynchrones
- Pagination des résultats
- Indexes DB optimisés
- Socket.io pour updates temps réel

## 🚦 État du Système

```
╔════════════════════════════════════════╗
║  KANGA HOLDING GROUP CCG - LIVE        ║
║  ✅ 3 Leaders IA (Alpha-Omega)        ║
║  ✅ 900 AI Betas autonomes            ║
║  ✅ 900 Divisions/Filiales            ║
║  ✅ Prospecting en direct activé      ║
║  ✅ Xenos (Générateur images) actif   ║
║  ✅ Système 100% autonome et live     ║
╚════════════════════════════════════════╝
```

## 📞 Support & Documentation

- **API Docs:** http://localhost:3000/docs
- **Logs:** `./logs/combined.log`
- **Issues:** GitHub Issues
- **Email:** support@kanga-holding.fr

## 📜 Licence

Propriétaire - Kanga Holding Group CCG - 2026

## 🎯 Prochaines Étapes

- [ ] Intégration Stripe pour paiements
- [ ] Dropshipping API connections
- [ ] SMS/Email campaigns automation
- [ ] Video generation with Xenos
- [ ] Advanced analytics dashboard
- [ ] Multi-currency support

---

**Créé avec ❤️ par Kanga Holding Group CCG**

*Système entièrement autonome. Les 903 IAs travaillent 24/7 pour générer des prospects et revenus.*