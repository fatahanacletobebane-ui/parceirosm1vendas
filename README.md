# Plataforma Publicidades & Cursos

## Estrutura do Projeto
- `index.html` - Website principal (usuários)
- `admin.html` - Consola de administração
- `firebase-rules.json` - Regras de segurança do Firebase

## Funcionalidades

### Para Utilizadores:
1. **Registo** com nome, telefone, email, PIN e código de referência opcional
2. **Login** com telefone + PIN (sem Firebase Auth)
3. **Partilha de Publicidades** - Ganhe 0.75 MTN por partilha (após aprovação admin)
4. **Código de Referência** - Ganhe 25 MTN por cada novo inscrito nas aulas
5. **FB Aulas Online** - Curso de 3 meses, 500 MTN (parcelado ou único)
6. **Madrassa Online** - Inscrição 150 MTN + mensalidade 100 MTN
7. **Sistema de Saldo** - Saldo principal + saldo de vendedor

### Para Administrador:
1. **Aprovação de Utilizadores** - Novos registos precisam de aprovação
2. **Aprovação de Partilhas** - Bónus só são atribuídos com aprovação
3. **Aprovação de Referências** - Comissões só com aprovação
4. **Gestão de Publicidades** - Adicionar/remover anúncios
5. **Gestão de Saldos** - Editar saldos manualmente
6. **Estatísticas** - Visão geral da plataforma

## Configuração Firebase

1. Acesse [Firebase Console](https://console.firebase.google.com)
2. Vá em "Realtime Database" → "Regras"
3. Cole o conteúdo de `firebase-rules.json`
4. Publique as regras

## Segurança

- Cada utilizador tem um UID único gerado automaticamente
- Senha de admin: `admin123` (alterar em produção!)
- Todas as transações de bónus/comissões requerem aprovação manual
- Sistema de referências rastreia quem convidou quem

## Contacto de Suporte
WhatsApp: 860407269 (link disponível na página de login)
