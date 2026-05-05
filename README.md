# 🌤️ Weather App - React Advanced

> Aplicação moderna de previsão do tempo com Context API e Custom Hooks

![Status](https://img.shields.io/badge/Status-Ativo-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)
![React](https://img.shields.io/badge/React-v18+-61DAFB?logo=react)
![API](https://img.shields.io/badge/API-OpenWeatherMap-orange)

## 📋 Visão Geral

Weather App é uma aplicação web moderna de previsão do tempo que demonstra padrões avançados de React como **Context API** e **Custom Hooks**. Permite:

- 🌍 Buscar previsão para qualquer cidade
- 📍 Localização automática por geolocalização
- 📅 Previsão para 7+ dias
- 🌡️ Dados detalhados (temperatura, umidade, vento, etc)
- 🌙 Modo automático claro/escuro
- 📱 Interface totalmente responsiva

## ✨ Funcionalidades Principais

- ✅ **Busca de Cidades** - Encontre previsão de qualquer lugar
- ✅ **Localização Automática** - Use sua localização atual
- ✅ **Previsão de 7 dias** - Veja o tempo dos próximos dias
- ✅ **Dados Detalhados** - Temperatura, umidade, vento, pressão
- ✅ **Ícones Dinâmicos** - Representação visual do clima
- ✅ **Context API** - State global sem prop drilling
- ✅ **Custom Hooks** - Lógica reutilizável
- ✅ **Histórico de Buscas** - Últimas cidades consultadas
- ✅ **Tema Claro/Escuro** - Confortável em qualquer hora
- ✅ **Responsivo** - Mobile, tablet e desktop
- ✅ **Sem Dependências Externas** - Apenas React puro

## 🛠️ Tecnologias Utilizadas

### Frontend
- **React 18** - Library UI moderna
- **React Hooks** - useState, useEffect, useContext, useCallback
- **Context API** - State management global
- **Custom Hooks** - useFetchWeather, useGeolocation, useLocalStorage
- **Vite** - Build tool rápido
- **CSS3** - Estilização com variáveis CSS

### API & Dados
- **OpenWeatherMap API** - Dados meteorológicos em tempo real
- **Geolocation API** - Localização do usuário
- **localStorage** - Persistência de dados

## 📁 Estrutura do Projeto

```
weather-app/
├── src/
│   ├── components/
│   │   ├── Header.jsx              # Cabeçalho e busca
│   │   ├── CurrentWeather.jsx      # Clima atual
│   │   ├── ForecastCard.jsx        # Card de previsão
│   │   ├── ForecastGrid.jsx        # Grid de 7 dias
│   │   ├── SearchBar.jsx           # Input de busca
│   │   ├── LocationButton.jsx      # Botão de localização
│   │   ├── ThemeToggle.jsx         # Toggle claro/escuro
│   │   └── LoadingSpinner.jsx      # Carregamento
│   │
│   ├── context/
│   │   └── WeatherContext.jsx      # Context API
│   │
│   ├── hooks/
│   │   ├── useFetchWeather.js      # Hook para buscar clima
│   │   ├── useGeolocation.js       # Hook para localização
│   │   └── useLocalStorage.js      # Hook para storage
│   │
│   ├── services/
│   │   └── weatherAPI.js           # Chamadas OpenWeatherMap
│   │
│   ├── utils/
│   │   ├── constants.js            # Constantes da app
│   │   ├── formatters.js           # Formatação de dados
│   │   └── icons.js                # Mapeamento de ícones
│   │
│   ├── styles/
│   │   ├── App.css
│   │   ├── components.css
│   │   ├── responsive.css
│   │   └── variables.css           # Variáveis CSS
│   │
│   ├── App.jsx
│   └── main.jsx
│
├── .env.example
├── package.json
└── README.md
```

## 🚀 Como Usar

### Pré-requisitos
- Node.js v16+
- npm ou yarn
- Chave API do OpenWeatherMap (gratuita)

### Instalação

#### 1. Clone o repositório
```bash
git clone https://github.com/ParreirasJuniorWeb/weather-app.git
cd weather-app
```

#### 2. Instale dependências
```bash
npm install
```

#### 3. Configure variáveis de ambiente
Crie `.env`:
```env
VITE_OPENWEATHER_API_KEY=sua_chave_aqui
VITE_API_BASE_URL=https://api.openweathermap.org/data/2.5
```

**Como obter a chave:**
1. Acesse [openweathermap.org](https://openweathermap.org/api)
2. Registre-se gratuitamente
3. Vá para "API Keys"
4. Copie a chave padrão

#### 4. Inicie o desenvolvimento
```bash
npm run dev
```

Acesse em: `http://localhost:5173`

## 💻 Scripts

```bash
npm run dev      # Desenvolvimento com hot reload
npm run build    # Build para produção
npm run preview  # Visualiza build local
npm run lint     # Verifica código (se configurado)
```

## 📚 Guia de Uso

### 1. Buscar uma Cidade
```
1. Digite o nome da cidade
2. Pressione Enter ou clique em Buscar
3. Aguarde o carregamento
4. Veja clima atual e previsão de 7 dias
```

### 2. Usar Localização Automática
```
1. Clique no botão 📍 "Minha Localização"
2. Permita acesso à localização
3. Clima local é carregado automaticamente
```

### 3. Ver Histórico de Buscas
```
1. Veja as últimas 5 cidades no dropdown
2. Clique para voltar a uma busca anterior
```

### 4. Alternar Tema
```
1. Clique no botão 🌙/☀️
2. Interface alterna entre claro e escuro
```

## 🎓 Conceitos Aprendidos

### Advanced React Patterns
- ✅ **Context API** - State global sem prop drilling
- ✅ **Custom Hooks** - Reutilização de lógica complexa
- ✅ **useContext + useReducer** - State management avançado
- ✅ **useCallback** - Otimização de performance
- ✅ **useEffect Cleanup** - Prevenção de memory leaks

### Fetching & Async
- ✅ **Fetch API** - Requisições HTTP
- ✅ **Async/Await** - Código síncrono com promises
- ✅ **Error Handling** - Tratamento robusto de erros
- ✅ **Loading States** - UX responsiva
- ✅ **API Caching** - Otimização de requisições

### Browser APIs
- ✅ **Geolocation API** - Latitude/Longitude do usuário
- ✅ **localStorage** - Persistência de dados
- ✅ **CSS Variables** - Temas dinâmicos

### Best Practices
- ✅ **Componentes Pequenos** - Single Responsibility
- ✅ **Separação de Concerns** - Logic vs UI
- ✅ **Variáveis de Ambiente** - Segurança de API keys
- ✅ **Error Boundaries** - Tratamento gracioso de erros

## 🪝 Custom Hooks Explicados

### `useFetchWeather`
```javascript
const { weather, loading, error } = useFetchWeather(city);
```
Busca dados do clima da API

### `useGeolocation`
```javascript
const { lat, lon, error } = useGeolocation();
```
Obtém coordenadas do usuário

### `useLocalStorage`
```javascript
const [searches, setSearches] = useLocalStorage('searches', []);
```
Persiste dados no localStorage

## 📊 Estrutura de Dados

### Clima Atual
```javascript
{
  city: "São Paulo",
  country: "BR",
  temp: 28,
  feelsLike: 30,
  humidity: 65,
  pressure: 1013,
  windSpeed: 5,
  cloudiness: 20,
  description: "Céu limpo",
  icon: "01d",
  sunrise: "06:30",
  sunset: "18:45"
}
```

### Previsão
```javascript
[
  {
    date: "2024-01-15",
    temp: 28,
    tempMin: 24,
    tempMax: 32,
    description: "Céu limpo",
    humidity: 65,
    windSpeed: 5
  }
]
```

## 🎨 Responsividade

### Breakpoints
- 📱 **Mobile** - < 640px (coluna única)
- 📲 **Tablet** - 640px - 1024px (2 colunas)
- 💻 **Desktop** - > 1024px (3+ colunas)

## 🔧 Troubleshooting

### Problema: "API Key inválida"
**Solução:** Verifique `.env`:
```bash
echo $VITE_OPENWEATHER_API_KEY
```

### Problema: "Localização bloqueada"
**Solução:** Permita acesso em configurações do navegador

### Problema: "Limite de requisições atingido"
**Solução:** OpenWeatherMap free tier permite 60 chamadas/minuto. Aguarde.

## 🚀 Deploy

### Vercel (Recomendado)
```bash
npm install -g vercel
vercel env add VITE_OPENWEATHER_API_KEY
vercel
```

### Netlify
```bash
npm run build
# Arraste pasta 'dist' no Netlify
# Configure variáveis em Site settings → Environment
```

### GitHub Pages
```bash
npm run build
git add dist/
git commit -m "Deploy"
git push
```

## 📝 Licença

MIT License - veja [LICENSE](LICENSE)

## 👨‍💻 Autor

**João Victor (Parreira Junior)**
- GitHub: [@ParreirasJuniorWeb](https://github.com/ParreirasJuniorWeb)

## 🎯 Roadmap

- [ ] Gráficos de previsão (Chart.js)
- [ ] Alertas de tempo severo
- [ ] Integração com mapas (Leaflet)
- [ ] Histórico de dados
- [ ] Modo offline
- [ ] PWA (Progressive Web App)
- [ ] Múltiplas cidades favoritas
- [ ] Compartilhamento de clima
- [ ] Notificações push

## 📚 Recursos Úteis

- [OpenWeatherMap Docs](https://openweathermap.org/api)
- [React Context](https://react.dev/reference/react/useContext)
- [React Custom Hooks](https://react.dev/learn/reusing-logic-with-custom-hooks)
- [Geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API)

---

⭐ Verifique o clima em qualquer lugar! ⭐