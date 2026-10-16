git init

cat > .gitignore <<'EOF'
.gradle/
build/
local.properties
.idea/
*.iml
.DS_Store

# Never commit signing credentials
*.keystore
*.jks
keystore.properties

# Secrets
.env
*.env
EOF

git add .
git commit -m "Initial LinguaGo translation app"

git branch -M main

git remote add origin https://github.com/FackOTP-debug/https-GGxLinguaGo.github.io.git

git push -u origin main
