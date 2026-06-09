# TreinoForte.com

Plataforma de gestão para personal trainers acompanharem seus clientes, treinos e agenda.

## Funcionalidades

- **Cadastro de clientes** — dados pessoais, histórico de saúde e medidas corporais
- **Planos de treino** — prescrição de exercícios organizados por grupos musculares
- **Registro de sessões** — FC repouso, FC média, FC máxima e percepção de esforço (escala de Borg/PSE)
- **Agenda** — horários disponíveis com valor por sessão e pagamento via PIX
- **Dashboard de evolução** — gráficos de progresso individual por cliente
- **Relatórios em PDF** — exportação do histórico de treinos e evolução

## Tecnologias

- [Next.js 14](https://nextjs.org/) (App Router)
- [Supabase](https://supabase.com/) (banco de dados PostgreSQL + autenticação)
- [Tailwind CSS](https://tailwindcss.com/)
- [Recharts](https://recharts.org/) (gráficos)
- [React PDF](https://react-pdf.org/) (geração de PDF)

## Como rodar localmente

**Pré-requisitos:** Node.js 20+, conta no Supabase

1. Clone o repositório:
   ```bash
   git clone https://github.com/JoaoPolo42/App-persona-trainer-TreinoForte.com.git
   cd App-persona-trainer-TreinoForte.com
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Configure as variáveis de ambiente — crie um arquivo `.env.local`:
   ```
   NEXT_PUBLIC_SUPABASE_URL=sua_url_do_supabase
   NEXT_PUBLIC_SUPABASE_ANON_KEY=sua_chave_anonima
   NEXT_PUBLIC_APP_PIX_KEY=sua_chave_pix
   NEXT_PUBLIC_APP_PIX_KEY_TYPE=email
   ```

4. Execute o banco de dados — rode o arquivo `supabase/schema.sql` no SQL Editor do Supabase.

5. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```
   Acesse em [http://localhost:3000](http://localhost:3000)

## Deploy

O projeto está configurado para deploy na [Vercel](https://vercel.com). Basta conectar o repositório e configurar as variáveis de ambiente.

## Licença

Uso privado — todos os direitos reservados.
