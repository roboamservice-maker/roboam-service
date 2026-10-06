# ROBOAM SERVICE — V12 (version consolidée V1→V11)

## Installation
1. `.env.example` → `.env` : URL Supabase + clé **publishable** (jamais service_role).
2. Supabase > SQL Editor : exécuter **`supabase_v12_complet.sql`** (un seul fichier, remplace tous les anciens SQL).
3. Créer un compte dans l'app, puis dans SQL Editor : `insert into public.admin_users(user_id) values('UUID_DU_COMPTE');`
4. `npm install` puis `npm run dev` (ou `npm run build`).

## Inclus
Catalogue, recherche, filtres, photos, favoris, avis, comptes, panier persistant, commande réelle (Supabase),
paiement à la livraison, mes commandes + suivi, administration (produits, statuts, paiements), choix Wave/Orange/MTN.

## Reste à faire
Paiement réel Wave/Orange/MTN (Edge Function + webhooks), vérification des prix côté serveur, upload photos, notifications, stock, codes promo, adresses multiples.
