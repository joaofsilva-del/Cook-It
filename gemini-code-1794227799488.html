import React, { useState, useEffect, useMemo, useRef } from 'react';
import { 
  Search, Heart, Clock, Utensils, Flame, Sparkles, Plus, Trash2, 
  CheckCircle2, Circle, ChefHat, ShoppingBag, Play, Pause, 
  RotateCcw, BookOpen, X, Check, Volume2, PlusCircle, CheckSquare,
  Award, ArrowRight, Refrigerator, Tag, RefreshCw, ChevronRight, Scale
} from 'lucide-react';

// Receitas pré-cadastradas completas
const INITIAL_RECIPES = [
  {
    id: '1',
    title: 'Bolo de Cenoura com Vulcão de Chocolate',
    category: 'Sobremesas',
    prepTime: 40,
    difficulty: 'Fácil',
    calories: 360,
    rating: 4.9,
    reviewsCount: 420,
    image: 'https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=800&q=80',
    description: 'Massa fofinha de cenoura batida no liquidificador com uma cobertura bem generosa e cremosa de brigadeiro gourmet.',
    basePortions: 4,
    ingredients: [
      { name: 'Cenouras médias descascadas', amount: 3, unit: 'unid' },
      { name: 'Óleo vegetal', amount: 120, unit: 'ml' },
      { name: 'Ovos', amount: 4, unit: 'unid' },
      { name: 'Açúcar refinado', amount: 300, unit: 'g' },
      { name: 'Farinha de Trigo', amount: 250, unit: 'g' },
      { name: 'Fermento em pó químico', amount: 1, unit: 'colher de sopa' },
      { name: 'Leite Condensado (para cobertura)', amount: 395, unit: 'g' },
      { name: 'Cacau em pó 50%', amount: 4, unit: 'colheres de sopa' },
      { name: 'Manteiga', amount: 1, unit: 'colher de sopa' }
    ],
    instructions: [
      'Bata as cenouras, os ovos e o óleo no liquidificador até obter um creme liso.',
      'Em uma tigela, misture a farinha e o açúcar. Despeje a mistura do liquidificador e mexa bem com um fouet.',
      'Adicione o fermento e misture delicadamente.',
      'Despeje numa forma untada e asse em forno pré-aquecido a 180°C por 40 minutos.',
      'Para a cobertura: leve ao fogo o leite condensado, o cacau e a manteiga até formar um brigadeiro mole.',
      'Desenforme o bolo e cubra com o brigadeiro ainda quente.'
    ],
    tags: ['Doces', 'Festa', 'Clássico']
  },
  {
    id: '2',
    title: 'Strogonoff de Frango Cremoso',
    category: 'Almoço/Jantar',
    prepTime: 25,
    difficulty: 'Fácil',
    calories: 410,
    rating: 4.9,
    reviewsCount: 310,
    image: 'https://images.unsplash.com/photo-1603894584373-5ac82b2ae398?auto=format&fit=crop&w=800&q=80',
    description: 'O clássico preferido de todos: tiras suculentas de frango em molho aveludado com cogumelos e batata palha.',
    basePortions: 4,
    ingredients: [
      { name: 'Peito de Frango cortado em cubos', amount: 500, unit: 'g' },
      { name: 'Creme de Leite', amount: 200, unit: 'g' },
      { name: 'Extrato de Tomate', amount: 3, unit: 'colheres de sopa' },
      { name: 'Ketchup', amount: 2, unit: 'colheres de sopa' },
      { name: 'Mostarda Amarela', amount: 1, unit: 'colher de sopa' },
      { name: 'Cogumelos Champignon fatiados', amount: 100, unit: 'g' },
      { name: 'Cebola picada', amount: 1, unit: 'unid' },
      { name: 'Alho picado', amount: 2, unit: 'dentes' },
      { name: 'Manteiga', amount: 2, unit: 'colheres de sopa' }
    ],
    instructions: [
      'Em uma panela, derreta a manteiga e doure a cebola e o alho.',
      'Adicione o frango em cubos e refogue até dourar bem.',
      'Junte os cogumelos, o extrato de tomate, o ketchup e a mostarda. Misture por 2 minutos.',
      'Abaixe o fogo, adicione o creme de leite e mexa bem sem deixar ferver.',
      'Sirva com arroz branco bem soltinho e batata palha crocante.'
    ],
    tags: ['Rápido', 'Prático', 'Favorito']
  },
  {
    id: '3',
    title: 'Risoto de Cogumelos Shimeji',
    category: 'Vegetarianas',
    prepTime: 30,
    difficulty: 'Médio',
    calories: 390,
    rating: 4.8,
    reviewsCount: 156,
    image: 'https://images.unsplash.com/photo-1633964913295-ceb43826e7c9?auto=format&fit=crop&w=800&q=80',
    description: 'Risoto italiano super cremoso, aromático com manteiga, vinho branco e cogumelos frescos salteados no alho.',
    basePortions: 2,
    ingredients: [
      { name: 'Arroz Arbóreo', amount: 200, unit: 'g' },
      { name: 'Cogumelo Shimeji', amount: 200, unit: 'g' },
      { name: 'Vinho Branco Seco', amount: 100, unit: 'ml' },
      { name: 'Caldo de Legumes aquecido', amount: 750, unit: 'ml' },
      { name: 'Cebola roxa picada', amount: 1, unit: 'unid' },
      { name: 'Queijo Parmesão ralado', amount: 60, unit: 'g' },
      { name: 'Manteiga gelada', amount: 2, unit: 'colheres de sopa' },
      { name: 'Azeite de oliva', amount: 2, unit: 'colheres de sopa' }
    ],
    instructions: [
      'Em uma frigideira, salteie o shimeji com um pouco de azeite e alho até murchar. Reserve.',
      'Em outra panela funda, refogue a cebola no azeite até ficar transparente.',
      'Adicione o arroz arbóreo e tostá-lo por 2 minutos. Adicione o vinho branco e mexa até evaporar.',
      'Vá adicionando o caldo de legumes quente aos poucos, concha por concha, mexendo sempre.',
      'Quando o arroz estiver al dente (aprox. 18 min), desligue o fogo.',
      'Incorpore os cogumelos reservados, o parmesão e a manteiga gelada para emulsionar.'
    ],
    tags: ['Gourmet', 'Vegetariano', 'Jantar Especial']
  },
  {
    id: '4',
    title: 'Panqueca Fit de Banana & Aveia',
    category: 'Fit/Saudável',
    prepTime: 12,
    difficulty: 'Fácil',
    calories: 210,
    rating: 4.75,
    reviewsCount: 289,
    image: 'https://images.unsplash.com/photo-1567620905732-2d1ec7ab7445?auto=format&fit=crop&w=800&q=80',
    description: 'Panqueca saudável, nutritiva e rápida para o café da manhã. Sem açúcar refinado e pronta em 10 minutos.',
    basePortions: 1,
    ingredients: [
      { name: 'Banana madura', amount: 1, unit: 'unid' },
      { name: 'Ovo', amount: 2, unit: 'unid' },
      { name: 'Farelo de Aveia', amount: 3, unit: 'colheres de sopa' },
      { name: 'Canela em pó', amount: 1, unit: 'pitada' },
      { name: 'Mel (opcional)', amount: 1, unit: 'colher de chá' }
    ],
    instructions: [
      'Em um prato, amasse bem a banana com um garfo.',
      'Adicione os ovos e bata bem até ficar homogêneo.',
      'Misture o farelo de aveia e a pitada de canela.',
      'Aqueça uma frigideira antiaderente levemente untada em fogo baixo.',
      'Despeje pequenas porções da massa, doure de um lado e vire cuidadosamente.',
      'Sirva com um fio de mel e rodelas de banana.'
    ],
    tags: ['Rápido', 'Fit', 'Café da Manhã']
  },
  {
    id: '5',
    title: 'Lasanha à Bolonhesa Tradicional',
    category: 'Almoço/Jantar',
    prepTime: 60,
    difficulty: 'Médio',
    calories: 520,
    rating: 4.9,
    reviewsCount: 380,
    image: 'https://images.unsplash.com/photo-1574894709920-11b28e7367e3?auto=format&fit=crop&w=800&q=80',
    description: 'Camadas generosas de massa para lasanha, molho de carne moída bem apurado, molho branco e muito queijo derretido.',
    basePortions: 6,
    ingredients: [
      { name: 'Massa para Lasanha', amount: 500, unit: 'g' },
      { name: 'Carne Moída (Patinho)', amount: 600, unit: 'g' },
      { name: 'Molho de Tomate', amount: 600, unit: 'g' },
      { name: 'Queijo Muçarela fatiado', amount: 400, unit: 'g' },
      { name: 'Presunto fatiado', amount: 300, unit: 'g' },
      { name: 'Leite', amount: 500, unit: 'ml' },
      { name: 'Farinha de Trigo', amount: 2, unit: 'colheres de sopa' },
      { name: 'Manteiga', amount: 2, unit: 'colheres de sopa' },
      { name: 'Cebola e Alho', amount: 1, unit: 'porção' }
    ],
    instructions: [
      'Refogue o alho e cebola, adicione a carne moída e doure. Adicione o molho de tomate e cozinhe por 15 min.',
      'Para o molho branco: derreta a manteiga, doure a farinha e adicione o leite aos poucos mexendo até engrossar.',
      'Em um refratário, faça uma camada de molho à bolonhesa, massa, presunto, muçarela e molho branco.',
      'Repita as camadas até o topo, finalizando com bastante queijo muçarela.',
      'Leve ao forno pré-aquecido a 200°C por 30 minutos até gratinar.'
    ],
    tags: ['Família', 'Domingo', 'Forno']
  },
  {
    id: '6',
    title: 'Feijoada Completa Brasileira',
    category: 'Almoço/Jantar',
    prepTime: 90,
    difficulty: 'Difícil',
    calories: 680,
    rating: 4.98,
    reviewsCount: 610,
    image: 'https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=800&q=80',
    description: 'A autêntica feijoada com feijão preto, carne seca, paia, calabresa e lombo suíno temperada com alho e louro.',
    basePortions: 8,
    ingredients: [
      { name: 'Feijão Preto', amount: 1, unit: 'kg' },
      { name: 'Carne Seca dessalgada', amount: 500, unit: 'g' },
      { name: 'Linguiça Calabresa', amount: 300, unit: 'g' },
      { name: 'Paiol / Bacon em cubos', amount: 200, unit: 'g' },
      { name: 'Costelinha de Porco', amount: 400, unit: 'g' },
      { name: 'Folhas de Louro', amount: 4, unit: 'unid' },
      { name: 'Alho picado', amount: 6, unit: 'dentes' },
      { name: 'Laranjas inteiras', amount: 2, unit: 'unid' }
    ],
    instructions: [
      'Cozinhe o feijão preto com as folhas de louro e as carnes duras na pressão por 30 minutos.',
      'Em uma frigideira grande, frite o bacon e a calabresa até dourarem.',
      'Adicione o alho picado à gordura do bacon e refogue bem.',
      'Junte esse refogado ao feijão com as carnes e adicione as laranjas cortadas ao meio (para amaciar).',
      'Cozinhe em fogo brando por mais 40 minutos até o caldo ficar bem encorpado.',
      'Sirva com couve refogada, farofa e torresmo.'
    ],
    tags: ['Tradição', 'Feijoada', 'Fim de Semana']
  },
  {
    id: '7',
    title: 'Frango Xadrez com Pimentões',
    category: 'Almoço/Jantar',
    prepTime: 20,
    difficulty: 'Fácil',
    calories: 340,
    rating: 4.82,
    reviewsCount: 204,
    image: 'https://images.unsplash.com/photo-1525755662778-989d0524087e?auto=format&fit=crop&w=800&q=80',
    description: 'Receita oriental com peito de frango macio, pimentões coloridos, amendoim crocante e molho Shoyu espesso.',
    basePortions: 4,
    ingredients: [
      { name: 'Peito de Frango em cubos', amount: 500, unit: 'g' },
      { name: 'Pimentão Vermelho em cubos', amount: 1, unit: 'unid' },
      { name: 'Pimentão Amarelo em cubos', amount: 1, unit: 'unid' },
      { name: 'Pimentão Verde em cubos', amount: 1, unit: 'unid' },
      { name: 'Cebola em cubos', amount: 1, unit: 'unid' },
      { name: 'Amendoim torrado sem pele', amount: 80, unit: 'g' },
      { name: 'Molho Shoyu', amount: 60, unit: 'ml' },
      { name: 'Amido de milho', amount: 1, unit: 'colher de sopa' }
    ],
    instructions: [
      'Em um wok ou frigideira grande, doure o frango no azeite até selar.',
      'Adicione a cebola e os pimentões coloridos e refogue rapidamente para manter a crocância.',
      'Dissolva o amido de milho no molho Shoyu com meio copo de água e adicione à frigideira.',
      'Mexa continuamente até o molho engrossar e envolver todos os ingredientes.',
      'Finalize com o amendoim torrado e sirva imediatamente.'
    ],
    tags: ['Rápido', 'Oriental', 'Colorido']
  },
  {
    id: '8',
    title: 'Tapioca de Frango com Requeijão',
    category: 'Fit/Saudável',
    prepTime: 10,
    difficulty: 'Fácil',
    calories: 260,
    rating: 4.88,
    reviewsCount: 195,
    image: 'https://images.unsplash.com/photo-1519708227418-c8fd9a32b7a2?auto=format&fit=crop&w=800&q=80',
    description: 'Tapioca crocante por fora e bem recheada com frango desfiado temperado e requeijão cremoso.',
    basePortions: 1,
    ingredients: [
      { name: 'Goma de Tapioca hidratada', amount: 100, unit: 'g' },
      { name: 'Frango desfiado temperado', amount: 80, unit: 'g' },
      { name: 'Requeijão cremoso', amount: 2, unit: 'colheres de sopa' },
      { name: 'Milho verde (opcional)', amount: 1, unit: 'colher de sopa' },
      { name: 'Orégano', amount: 1, unit: 'pitada' }
    ],
    instructions: [
      'Peneire a goma de tapioca diretamente em uma frigideira antiaderente bem aquecida.',
      'Espalhe uniformemente formando um disco e deixe cozinhar por cerca de 2 minutos até soltar da borda.',
      'Espalhe o requeijão cremoso em metade da tapioca.',
      'Adicione o frango desfiado, o milho e salpique orégano.',
      'Dobre ao meio e deixe mais 30 segundos de cada lado para aquecer o recheio.'
    ],
    tags: ['Rápido', 'Sem Glúten', 'Lanche']
  }
];

export default function App() {
  // Navigation State
  const [activeTab, setActiveTab] = useState('recipes'); // 'recipes', 'fridge', 'shopping', 'create'
  
  // Storage & Core Data States
  const [recipes, setRecipes] = useState(() => {
    const saved = localStorage.getItem('cookit_recipes_v2');
    return saved ? JSON.parse(saved) : INITIAL_RECIPES;
  });
  
  const [favorites, setFavorites] = useState(() => {
    const saved = localStorage.getItem('cookit_favorites');
    return saved ? JSON.parse(saved) : ['1', '2'];
  });

  const [shoppingList, setShoppingList] = useState(() => {
    const saved = localStorage.getItem('cookit_shopping');
    return saved ? JSON.parse(saved) : [
      { id: '1', name: 'Leite Condensado', amount: '1 lata', completed: false },
      { id: '2', name: 'Ovos', amount: '1 dúzia', completed: true },
      { id: '3', name: 'Peito de Frango', amount: '1 kg', completed: false }
    ];
  });

  // Filter States
  const [searchQuery, setSearchQuery] = useState('');
  const [selectedCategory, setSelectedCategory] = useState('Todas');
  const [onlyFavorites, setOnlyFavorites] = useState(false);

  // Selected Recipe Modal / Detail view
  const [selectedRecipe, setSelectedRecipe] = useState(null);
  const [scaledPortions, setScaledPortions] = useState(4);
  const [checkedSteps, setCheckedSteps] = useState({});

  // Timer State
  const [timerSeconds, setTimerSeconds] = useState(0);
  const [timerInitial, setTimerInitial] = useState(0);
  const [timerActive, setTimerActive] = useState(false);

  // Fridge Matcher State
  const [selectedFridgeIngredients, setSelectedFridgeIngredients] = useState([]);
  const [customFridgeItem, setCustomFridgeItem] = useState('');

  // Save changes to LocalStorage
  useEffect(() => {
    localStorage.setItem('cookit_recipes_v2', JSON.stringify(recipes));
  }, [recipes]);

  useEffect(() => {
    localStorage.setItem('cookit_favorites', JSON.stringify(favorites));
  }, [favorites]);

  useEffect(() => {
    localStorage.setItem('cookit_shopping', JSON.stringify(shoppingList));
  }, [shoppingList]);

  // Audio Beep generator using Web Audio API for timer completion
  const playTimerSound = () => {
    try {
      const audioCtx = new (window.AudioContext || window.webkitAudioContext)();
      const osc = audioCtx.createOscillator();
      const gain = audioCtx.createGain();
      osc.type = 'sine';
      osc.frequency.setValueAtTime(587.33, audioCtx.currentTime); // D5
      gain.gain.setValueAtTime(0.1, audioCtx.currentTime);
      osc.connect(gain);
      gain.connect(audioCtx.destination);
      osc.start();
      osc.stop(audioCtx.currentTime + 1.2);
    } catch (e) {
      console.log('Audio Context Error', e);
    }
  };

  // Kitchen Timer interval logic
  useEffect(() => {
    let interval = null;
    if (timerActive && timerSeconds > 0) {
      interval = setInterval(() => {
        setTimerSeconds(sec => sec - 1);
      }, 1000);
    } else if (timerSeconds === 0 && timerActive) {
      setTimerActive(false);
      playTimerSound();
    }
    return () => clearInterval(interval);
  }, [timerActive, timerSeconds]);

  // Helper function to format seconds to MM:SS
  const formatTime = (secs) => {
    const m = Math.floor(secs / 60);
    const s = secs % 60;
    return `${m.toString().padStart(2, '0')}:${s.toString().padStart(2, '0')}`;
  };

  const startTimer = (minutes) => {
    const totalSecs = minutes * 60;
    setTimerInitial(totalSecs);
    setTimerSeconds(totalSecs);
    setTimerActive(true);
  };

  // Toggle Favorite
  const toggleFavorite = (id, e) => {
    if (e) e.stopPropagation();
    setFavorites(prev => 
      prev.includes(id) ? prev.filter(item => item !== id) : [...prev, id]
    );
  };

  // Open recipe modal and set base portions
  const openRecipe = (recipe) => {
    setSelectedRecipe(recipe);
    setScaledPortions(recipe.basePortions || 4);
    setCheckedSteps({});
  };

  // Add all recipe ingredients to shopping list
  const addRecipeToShoppingList = (recipe, portions) => {
    const ratio = portions / (recipe.basePortions || 4);
    const newItems = recipe.ingredients.map(ing => ({
      id: Date.now() + Math.random().toString(),
      name: ing.name,
      amount: `${(ing.amount * ratio).toFixed(1).replace('.0', '')} ${ing.unit}`,
      completed: false
    }));
    setShoppingList(prev => [...prev, ...newItems]);
  };

  // Filtered recipes
  const filteredRecipes = useMemo(() => {
    return recipes.filter(recipe => {
      const matchesSearch = recipe.title.toLowerCase().includes(searchQuery.toLowerCase()) ||
        recipe.ingredients.some(i => i.name.toLowerCase().includes(searchQuery.toLowerCase())) ||
        recipe.tags.some(t => t.toLowerCase().includes(searchQuery.toLowerCase()));

      const matchesCategory = selectedCategory === 'Todas' || 
        (selectedCategory === 'Rápida (< 30min)' && recipe.prepTime <= 30) ||
        recipe.category === selectedCategory;

      const matchesFav = !onlyFavorites || favorites.includes(recipe.id);

      return matchesSearch && matchesCategory && matchesFav;
    });
  }, [recipes, searchQuery, selectedCategory, onlyFavorites, favorites]);

  // Common fridge ingredient list for quick selection
  const commonIngredients = ['Ovos', 'Leite', 'Frango', 'Cenoura', 'Arroz', 'Manteiga', 'Alho', 'Cebola', 'Creme de Leite', 'Queijo', 'Tomate', 'Farinha de Trigo'];

  // Fridge matcher calculation
  const fridgeMatches = useMemo(() => {
    if (selectedFridgeIngredients.length === 0) return [];
    
    return recipes.map(recipe => {
      const recipeIngNames = recipe.ingredients.map(i => i.name.toLowerCase());
      const matched = selectedFridgeIngredients.filter(userIng => 
        recipeIngNames.some(rIng => rIng.includes(userIng.toLowerCase()))
      );
      const matchPercentage = Math.round((matched.length / recipe.ingredients.length) * 100);

      return {
        ...recipe,
        matchedCount: matched.length,
        matchedIngredients: matched,
        matchPercentage
      };
    }).filter(item => item.matchedCount > 0)
      .sort((a, b) => b.matchPercentage - a.matchPercentage);
  }, [recipes, selectedFridgeIngredients]);

  return (
    <div className="min-h-screen bg-[#FAF6F0] text-stone-800 font-sans flex flex-col selection:bg-orange-200">
      
      {/* HEADER / NAVIGATION BAR */}
      <header className="sticky top-0 z-30 bg-white border-b border-orange-100 shadow-sm">
        <div className="max-w-6xl mx-auto px-4 sm:px-6 h-16 flex items-center justify-between">
          <div className="flex items-center space-x-3 cursor-pointer" onClick={() => setActiveTab('recipes')}>
            <div className="w-10 h-10 rounded-xl bg-gradient-to-tr from-[#E05638] to-orange-400 flex items-center justify-center text-white shadow-md shadow-orange-200">
              <ChefHat size={24} />
            </div>
            <div>
              <span className="text-xl font-bold tracking-tight bg-gradient-to-r from-[#E05638] to-amber-700 bg-clip-text text-transparent">
                CookIt
              </span>
              <span className="hidden sm:inline-block text-xs text-amber-700 font-medium ml-2 px-2 py-0.5 bg-orange-100 rounded-full">
                Sabor & Praticidade
              </span>
            </div>
          </div>

          {/* Desktop Navigation */}
          <nav className="hidden md:flex items-center space-x-1">
            <button
              onClick={() => setActiveTab('recipes')}
              className={`px-4 py-2 rounded-xl text-sm font-medium transition-all flex items-center gap-2 ${
                activeTab === 'recipes' 
                  ? 'bg-orange-50 text-[#E05638] font-semibold' 
                  : 'text-stone-600 hover:text-stone-900 hover:bg-stone-100'
              }`}
            >
              <BookOpen size={18} /> Receitas
            </button>
            <button
              onClick={() => setActiveTab('fridge')}
              className={`px-4 py-2 rounded-xl text-sm font-medium transition-all flex items-center gap-2 ${
                activeTab === 'fridge' 
                  ? 'bg-orange-50 text-[#E05638] font-semibold' 
                  : 'text-stone-600 hover:text-stone-900 hover:bg-stone-100'
              }`}
            >
              <Refrigerator size={18} /> O Que Tem Na Geladeira?
            </button>
            <button
              onClick={() => setActiveTab('shopping')}
              className={`px-4 py-2 rounded-xl text-sm font-medium transition-all flex items-center gap-2 relative ${
                activeTab === 'shopping' 
                  ? 'bg-orange-50 text-[#E05638] font-semibold' 
                  : 'text-stone-600 hover:text-stone-900 hover:bg-stone-100'
              }`}
            >
              <ShoppingBag size={18} /> Lista de Compras
              {shoppingList.filter(i => !i.completed).length > 0 && (
                <span className="w-5 h-5 bg-[#E05638] text-white text-xs font-bold rounded-full flex items-center justify-center">
                  {shoppingList.filter(i => !i.completed).length}
                </span>
              )}
            </button>
          </nav>

          {/* Action Buttons */}
          <div className="flex items-center space-x-2">
            <button
              onClick={() => setActiveTab('create')}
              className="bg-[#E05638] hover:bg-[#c9452a] text-white px-4 py-2 rounded-xl text-sm font-medium transition-all flex items-center gap-1.5 shadow-sm shadow-orange-300 active:scale-95"
            >
              <Plus size={18} /> 
              <span className="hidden sm:inline">Nova Receita</span>
            </button>
          </div>
        </div>

        {/* Mobile Navigation Bar */}
        <div className="md:hidden flex border-t border-stone-200 bg-white px-2 py-1 justify-around">
          <button
            onClick={() => setActiveTab('recipes')}
            className={`flex flex-col items-center py-1.5 px-3 rounded-lg text-xs font-medium ${
              activeTab === 'recipes' ? 'text-[#E05638]' : 'text-stone-500'
            }`}
          >
            <BookOpen size={18} />
            Receitas
          </button>
          <button
            onClick={() => setActiveTab('fridge')}
            className={`flex flex-col items-center py-1.5 px-3 rounded-lg text-xs font-medium ${
              activeTab === 'fridge' ? 'text-[#E05638]' : 'text-stone-500'
            }`}
          >
            <Refrigerator size={18} />
            Geladeira
          </button>
          <button
            onClick={() => setActiveTab('shopping')}
            className={`flex flex-col items-center py-1.5 px-3 rounded-lg text-xs font-medium relative ${
              activeTab === 'shopping' ? 'text-[#E05638]' : 'text-stone-500'
            }`}
          >
            <ShoppingBag size={18} />
            Compras
            {shoppingList.filter(i => !i.completed).length > 0 && (
              <span className="absolute top-1 right-2 w-2 h-2 bg-[#E05638] rounded-full"></span>
            )}
          </button>
        </div>
      </header>

      {/* TIMER FLOATING BAR (If active or running) */}
      {timerSeconds > 0 && (
        <div className="bg-[#2E7D32] text-white px-4 py-2.5 shadow-lg flex items-center justify-between z-20 text-sm">
          <div className="flex items-center gap-2 max-w-6xl mx-auto w-full justify-between">
            <div className="flex items-center gap-2">
              <Clock className="animate-pulse" size={18} />
              <span className="font-medium">Timer da Cozinha:</span>
              <span className="font-mono text-lg font-bold bg-emerald-900/40 px-2 py-0.5 rounded">
                {formatTime(timerSeconds)}
              </span>
            </div>
            <div className="flex items-center gap-2">
              <button 
                onClick={() => setTimerActive(!timerActive)}
                className="bg-white/20 hover:bg-white/30 px-3 py-1 rounded-lg text-xs font-medium transition"
              >
                {timerActive ? <Pause size={14} /> : <Play size={14} />}
              </button>
              <button 
                onClick={() => { setTimerSeconds(0); setTimerActive(false); }}
                className="bg-white/20 hover:bg-white/30 px-3 py-1 rounded-lg text-xs font-medium transition"
              >
                <X size={14} />
              </button>
            </div>
          </div>
        </div>
      )}

      {/* MAIN CONTENT AREA */}
      <main className="max-w-6xl mx-auto px-4 sm:px-6 py-6 flex-1 w-full">
        
        {/* VIEW 1: RECIPES FEED & SEARCH */}
        {activeTab === 'recipes' && (
          <div className="space-y-6">
            
            {/* HERO BANNER & SEARCH */}
            <div className="bg-gradient-to-r from-[#E05638] via-amber-600 to-orange-500 rounded-3xl p-6 sm:p-10 text-white shadow-xl relative overflow-hidden">
              <div className="absolute right-0 bottom-0 opacity-10 pointer-events-none transform translate-x-10 translate-y-10">
                <ChefHat size={280} />
              </div>
              <div className="max-w-xl relative z-10 space-y-3">
                <span className="inline-flex items-center gap-1.5 bg-white/20 backdrop-blur-md px-3 py-1 rounded-full text-xs font-medium">
                  <Sparkles size={14} /> O que vamos cozinhar hoje?
                </span>
                <h1 className="text-2xl sm:text-4xl font-extrabold tracking-tight leading-tight">
                  Descubra receitas fáceis, deliciosas e sob medida.
                </h1>
                <p className="text-orange-100 text-sm sm:text-base">
                  Cozinhe como um chef com porcionador automático de ingredientes e timer inteligente.
                </p>

                {/* SEARCH BAR */}
                <div className="pt-2">
                  <div className="relative flex items-center bg-white text-stone-800 rounded-2xl shadow-lg overflow-hidden">
                    <Search size={20} className="ml-4 text-stone-400" />
                    <input
                      type="text"
                      placeholder="Busque por título, ingrediente (ex: frango, chocolate)..."
                      value={searchQuery}
                      onChange={(e) => setSearchQuery(e.target.value)}
                      className="w-full px-4 py-3.5 text-sm sm:text-base outline-none border-none placeholder-stone-400"
                    />
                    {searchQuery && (
                      <button 
                        onClick={() => setSearchQuery('')}
                        className="p-2 mr-2 text-stone-400 hover:text-stone-600"
                      >
                        <X size={18} />
                      </button>
                    )}
                  </div>
                </div>
              </div>
            </div>

            {/* FILTERS & CATEGORIES */}
            <div className="flex flex-col sm:flex-row sm:items-center justify-between gap-4">
              <div className="flex items-center gap-2 overflow-x-auto pb-2 sm:pb-0 no-scrollbar">
                {['Todas', 'Rápida (< 30min)', 'Almoço/Jantar', 'Sobremesas', 'Fit/Saudável', 'Vegetarianas'].map(cat => (
                  <button
                    key={cat}
                    onClick={() => setSelectedCategory(cat)}
                    className={`px-4 py-2 rounded-xl text-xs sm:text-sm font-medium whitespace-nowrap transition-all ${
                      selectedCategory === cat
                        ? 'bg-[#E05638] text-white shadow-md shadow-orange-200 font-semibold'
                        : 'bg-white text-stone-600 hover:bg-stone-100 border border-stone-200/80'
                    }`}
                  >
                    {cat}
                  </button>
                ))}
              </div>

              {/* Favorites toggle */}
              <button
                onClick={() => setOnlyFavorites(!onlyFavorites)}
                className={`px-4 py-2 rounded-xl text-xs sm:text-sm font-medium flex items-center gap-2 border transition-all ${
                  onlyFavorites
                    ? 'bg-rose-50 border-rose-300 text-rose-600 font-semibold'
                    : 'bg-white border-stone-200 text-stone-600 hover:bg-stone-50'
                }`}
              >
                <Heart size={16} className={onlyFavorites ? 'fill-rose-500 text-rose-500' : ''} />
                Favoritas ({favorites.length})
              </button>
            </div>

            {/* RECIPES GRID */}
            {filteredRecipes.length === 0 ? (
              <div className="bg-white rounded-3xl p-12 text-center border border-dashed border-stone-300 my-8">
                <Utensils size={48} className="mx-auto text-stone-300 mb-3" />
                <h3 className="text-lg font-bold text-stone-700">Nenhuma receita encontrada</h3>
                <p className="text-stone-500 text-sm mt-1">Tente mudar o termo da busca ou ajustar os filtros de categoria.</p>
                <button
                  onClick={() => { setSearchQuery(''); setSelectedCategory('Todas'); setOnlyFavorites(false); }}
                  className="mt-4 px-4 py-2 bg-stone-100 hover:bg-stone-200 text-stone-700 rounded-xl text-xs font-semibold"
                >
                  Limpar todos os filtros
                </button>
              </div>
            ) : (
              <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                {filteredRecipes.map(recipe => (
                  <div
                    key={recipe.id}
                    onClick={() => openRecipe(recipe)}
                    className="bg-white rounded-2xl overflow-hidden border border-stone-200/80 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col cursor-pointer group hover:-translate-y-1"
                  >
                    {/* Image Banner */}
                    <div className="relative h-48 overflow-hidden bg-stone-100">
                      <img 
                        src={recipe.image} 
                        alt={recipe.title} 
                        className="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500"
                        loading="lazy"
                      />
                      <div className="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-60"></div>
                      
                      {/* Top Badges */}
                      <span className="absolute top-3 left-3 bg-white/90 backdrop-blur-md text-stone-800 text-xs px-2.5 py-1 rounded-full font-semibold shadow-sm">
                        {recipe.category}
                      </span>
                      
                      <button
                        onClick={(e) => toggleFavorite(recipe.id, e)}
                        className="absolute top-3 right-3 p-2 bg-white/80 backdrop-blur-md rounded-full text-stone-700 hover:text-rose-500 hover:bg-white transition"
                      >
                        <Heart 
                          size={18} 
                          className={favorites.includes(recipe.id) ? 'fill-rose-500 text-rose-500' : ''} 
                        />
                      </button>

                      {/* Prep time badge */}
                      <div className="absolute bottom-3 left-3 flex items-center gap-1 text-white text-xs font-medium">
                        <Clock size={14} />
                        {recipe.prepTime} min
                      </div>
                    </div>

                    {/* Recipe Details */}
                    <div className="p-5 flex-1 flex flex-col justify-between space-y-3">
                      <div>
                        <div className="flex items-center gap-2 text-xs text-amber-600 font-medium mb-1">
                          <span className="flex items-center gap-0.5">
                            ★ {recipe.rating}
                          </span>
                          <span>•</span>
                          <span>{recipe.difficulty}</span>
                          <span>•</span>
                          <span>{recipe.calories} kcal</span>
                        </div>
                        <h3 className="font-bold text-lg text-stone-800 group-hover:text-[#E05638] transition-colors line-clamp-1">
                          {recipe.title}
                        </h3>
                        <p className="text-stone-500 text-xs mt-1.5 line-clamp-2 leading-relaxed">
                          {recipe.description}
                        </p>
                      </div>

                      {/* Tags */}
                      <div className="pt-2 border-t border-stone-100 flex items-center justify-between">
                        <div className="flex flex-wrap gap-1">
                          {recipe.tags.slice(0, 2).map((t, idx) => (
                            <span key={idx} className="bg-stone-100 text-stone-600 text-[10px] px-2 py-0.5 rounded-md">
                              #{t}
                            </span>
                          ))}
                        </div>
                        <span className="text-[#E05638] font-bold text-xs flex items-center gap-0.5 group-hover:translate-x-1 transition-transform">
                          Ver Receita <ChevronRight size={14} />
                        </span>
                      </div>
                    </div>
                  </div>
                ))}
              </div>
            )}
          </div>
        )}

        {/* VIEW 2: FRIDGE MATCHER */}
        {activeTab === 'fridge' && (
          <div className="max-w-4xl mx-auto space-y-6">
            <div className="bg-white rounded-3xl p-6 sm:p-8 border border-stone-200/80 shadow-sm space-y-6">
              <div className="flex items-start gap-4">
                <div className="p-3 bg-emerald-100 text-[#2E7D32] rounded-2xl">
                  <Refrigerator size={32} />
                </div>
                <div>
                  <h2 className="text-xl sm:text-2xl font-bold text-stone-800">O Que Tem Na Geladeira?</h2>
                  <p className="text-stone-500 text-sm mt-1">
                    Selecione os ingredientes que você possui em casa para encontrarmos as melhores receitas compatíveis.
                  </p>
                </div>
              </div>

              {/* Quick ingredient badges */}
              <div className="space-y-3">
                <label className="text-xs font-bold text-stone-600 uppercase tracking-wider">
                  Ingredientes rápidos (Clique para selecionar):
                </label>
                <div className="flex flex-wrap gap-2">
                  {commonIngredients.map(ing => {
                    const isSelected = selectedFridgeIngredients.includes(ing);
                    return (
                      <button
                        key={ing}
                        onClick={() => {
                          setSelectedFridgeIngredients(prev => 
                            isSelected ? prev.filter(i => i !== ing) : [...prev, ing]
                          );
                        }}
                        className={`px-3.5 py-1.5 rounded-xl text-xs font-medium transition-all flex items-center gap-1.5 ${
                          isSelected
                            ? 'bg-[#2E7D32] text-white shadow-sm font-semibold'
                            : 'bg-stone-100 text-stone-700 hover:bg-stone-200'
                        }`}
                      >
                        {isSelected && <Check size={14} />}
                        {ing}
                      </button>
                    );
                  })}
                </div>
              </div>

              {/* Custom ingredient input */}
              <div className="flex gap-2 pt-2">
                <input
                  type="text"
                  placeholder="Ou adicione outro ingrediente..."
                  value={customFridgeItem}
                  onChange={(e) => setCustomFridgeItem(e.target.value)}
                  onKeyDown={(e) => {
                    if (e.key === 'Enter' && customFridgeItem.trim()) {
                      if (!selectedFridgeIngredients.includes(customFridgeItem.trim())) {
                        setSelectedFridgeIngredients([...selectedFridgeIngredients, customFridgeItem.trim()]);
                      }
                      setCustomFridgeItem('');
                    }
                  }}
                  className="flex-1 px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#2E7D32]"
                />
                <button
                  onClick={() => {
                    if (customFridgeItem.trim()) {
                      if (!selectedFridgeIngredients.includes(customFridgeItem.trim())) {
                        setSelectedFridgeIngredients([...selectedFridgeIngredients, customFridgeItem.trim()]);
                      }
                      setCustomFridgeItem('');
                    }
                  }}
                  className="bg-[#2E7D32] text-white px-4 py-2 rounded-xl text-xs font-semibold hover:bg-emerald-800 transition"
                >
                  Adicionar
                </button>
              </div>

              {/* Active selections */}
              {selectedFridgeIngredients.length > 0 && (
                <div className="pt-3 border-t border-stone-100 flex items-center justify-between">
                  <span className="text-xs text-stone-500">
                    {selectedFridgeIngredients.length} ingredientes selecionados
                  </span>
                  <button 
                    onClick={() => setSelectedFridgeIngredients([])}
                    className="text-xs text-rose-500 hover:underline"
                  >
                    Limpar seleção
                  </button>
                </div>
              )}
            </div>

            {/* Match Results */}
            <div className="space-y-4">
              <h3 className="font-bold text-lg text-stone-800">
                {selectedFridgeIngredients.length === 0 
                  ? 'Selecione ingredientes acima para ver sugestões'
                  : `Receitas encontradas (${fridgeMatches.length})`}
              </h3>

              {selectedFridgeIngredients.length > 0 && fridgeMatches.length === 0 && (
                <div className="bg-white rounded-2xl p-8 text-center text-stone-500 border border-stone-200">
                  Nenhuma receita encontrada com esses ingredientes exatos. Tente adicionar mais itens como cebola, alho ou ovos.
                </div>
              )}

              <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                {fridgeMatches.map(recipe => (
                  <div
                    key={recipe.id}
                    onClick={() => openRecipe(recipe)}
                    className="bg-white rounded-2xl p-4 border border-stone-200/80 shadow-sm hover:shadow-md transition flex gap-4 cursor-pointer"
                  >
                    <img 
                      src={recipe.image} 
                      alt={recipe.title} 
                      className="w-24 h-24 rounded-xl object-cover"
                    />
                    <div className="flex-1 flex flex-col justify-between">
                      <div>
                        <div className="flex items-center justify-between">
                          <span className="text-xs font-bold text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded-md">
                            {recipe.matchPercentage}% de Match
                          </span>
                          <span className="text-xs text-stone-400">{recipe.prepTime} min</span>
                        </div>
                        <h4 className="font-bold text-stone-800 mt-1 line-clamp-1">{recipe.title}</h4>
                        <p className="text-xs text-stone-500 mt-1">
                          Você tem: <strong className="text-stone-700">{recipe.matchedIngredients.join(', ')}</strong>
                        </p>
                      </div>

                      <span className="text-[#E05638] text-xs font-bold flex items-center gap-1 mt-2">
                        Ver Receita <ArrowRight size={12} />
                      </span>
                    </div>
                  </div>
                ))}
              </div>
            </div>
          </div>
        )}

        {/* VIEW 3: SHOPPING LIST */}
        {activeTab === 'shopping' && (
          <div className="max-w-3xl mx-auto space-y-6">
            <div className="bg-white rounded-3xl p-6 sm:p-8 border border-stone-200/80 shadow-sm space-y-6">
              <div className="flex items-center justify-between">
                <div className="flex items-center gap-3">
                  <div className="p-3 bg-orange-100 text-[#E05638] rounded-2xl">
                    <ShoppingBag size={28} />
                  </div>
                  <div>
                    <h2 className="text-xl font-bold text-stone-800">Lista de Compras</h2>
                    <p className="text-xs text-stone-500">Marque os itens à medida que for comprando no supermercado.</p>
                  </div>
                </div>

                {shoppingList.length > 0 && (
                  <button
                    onClick={() => setShoppingList([])}
                    className="text-xs text-rose-500 hover:underline font-medium"
                  >
                    Limpar Tudo
                  </button>
                )}
              </div>

              {/* Add Custom Shopping Item */}
              <form 
                onSubmit={(e) => {
                  e.preventDefault();
                  const form = e.target;
                  const name = form.itemName.value.trim();
                  const amount = form.itemAmount.value.trim();
                  if (name) {
                    setShoppingList(prev => [
                      ...prev, 
                      { id: Date.now().toString(), name, amount: amount || '1 unid', completed: false }
                    ]);
                    form.reset();
                  }
                }}
                className="flex gap-2"
              >
                <input
                  name="itemName"
                  type="text"
                  placeholder="Nome do item (ex: Queijo Parmesão)"
                  required
                  className="flex-1 px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                />
                <input
                  name="itemAmount"
                  type="text"
                  placeholder="Qtd (ex: 200g)"
                  className="w-28 px-3 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                />
                <button
                  type="submit"
                  className="bg-[#E05638] hover:bg-[#c9452a] text-white px-4 py-2.5 rounded-xl text-xs font-semibold transition"
                >
                  <Plus size={18} />
                </button>
              </form>

              {/* Items List */}
              <div className="space-y-2 pt-2">
                {shoppingList.length === 0 ? (
                  <p className="text-center text-stone-400 text-sm py-8">
                    Sua lista de compras está vazia. Adicione itens ou clique em "Adicionar à Lista de Compras" dentro de uma receita!
                  </p>
                ) : (
                  shoppingList.map(item => (
                    <div
                      key={item.id}
                      className={`flex items-center justify-between p-3.5 rounded-xl border transition ${
                        item.completed 
                          ? 'bg-stone-50 border-stone-200 text-stone-400 line-through' 
                          : 'bg-white border-stone-200 text-stone-800 hover:border-orange-200'
                      }`}
                    >
                      <div 
                        onClick={() => {
                          setShoppingList(prev => prev.map(i => i.id === item.id ? { ...i, completed: !i.completed } : i));
                        }}
                        className="flex items-center gap-3 cursor-pointer flex-1"
                      >
                        {item.completed ? (
                          <CheckCircle2 size={20} className="text-emerald-500" />
                        ) : (
                          <Circle size={20} className="text-stone-300" />
                        )}
                        <span className="text-sm font-medium">{item.name}</span>
                        {item.amount && (
                          <span className="text-xs bg-stone-100 text-stone-500 px-2 py-0.5 rounded-md ml-auto mr-4">
                            {item.amount}
                          </span>
                        )}
                      </div>

                      <button
                        onClick={() => setShoppingList(prev => prev.filter(i => i.id !== item.id))}
                        className="text-stone-300 hover:text-rose-500 transition p-1"
                      >
                        <Trash2 size={16} />
                      </button>
                    </div>
                  ))
                )}
              </div>
            </div>
          </div>
        )}

        {/* VIEW 4: CREATE RECIPE */}
        {activeTab === 'create' && (
          <div className="max-w-3xl mx-auto space-y-6">
            <div className="bg-white rounded-3xl p-6 sm:p-8 border border-stone-200/80 shadow-sm space-y-6">
              <div className="flex items-center justify-between border-b border-stone-100 pb-4">
                <div>
                  <h2 className="text-2xl font-bold text-stone-800">Cadastrar Nova Receita</h2>
                  <p className="text-stone-500 text-xs mt-0.5">Adicione sua receita exclusiva ao seu livro digital do CookIt.</p>
                </div>
                <button 
                  onClick={() => setActiveTab('recipes')}
                  className="p-2 text-stone-400 hover:text-stone-600 rounded-full hover:bg-stone-100"
                >
                  <X size={20} />
                </button>
              </div>

              <form 
                onSubmit={(e) => {
                  e.preventDefault();
                  const form = e.target;
                  
                  const title = form.recipeTitle.value;
                  const category = form.recipeCategory.value;
                  const prepTime = parseInt(form.recipeTime.value) || 30;
                  const difficulty = form.recipeDifficulty.value;
                  const image = form.recipeImage.value || 'https://images.unsplash.com/photo-1495521821757-a1efb6729352?auto=format&fit=crop&w=800&q=80';
                  const description = form.recipeDesc.value;

                  // Parse ingredients text area (Line by line)
                  const rawIngs = form.recipeIngredientsText.value.split('\n');
                  const parsedIngs = rawIngs.filter(line => line.trim()).map(line => ({
                    name: line.trim(),
                    amount: 1,
                    unit: 'porção'
                  }));

                  // Parse steps
                  const rawSteps = form.recipeStepsText.value.split('\n');
                  const parsedSteps = rawSteps.filter(line => line.trim());

                  const newRecipeObj = {
                    id: Date.now().toString(),
                    title,
                    category,
                    prepTime,
                    difficulty,
                    calories: 350,
                    rating: 5.0,
                    reviewsCount: 1,
                    image,
                    description,
                    basePortions: 4,
                    ingredients: parsedIngs,
                    instructions: parsedSteps,
                    tags: ['Minha Receita', category]
                  };

                  setRecipes(prev => [newRecipeObj, ...prev]);
                  setActiveTab('recipes');
                  openRecipe(newRecipeObj);
                }}
                className="space-y-4"
              >
                <div>
                  <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Título da Receita *</label>
                  <input
                    name="recipeTitle"
                    type="text"
                    required
                    placeholder="Ex: Torta de Frango Prática"
                    className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                  />
                </div>

                <div className="grid grid-cols-1 sm:grid-cols-3 gap-4">
                  <div>
                    <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Categoria</label>
                    <select 
                      name="recipeCategory" 
                      className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                    >
                      <option>Almoço/Jantar</option>
                      <option>Sobremesas</option>
                      <option>Fit/Saudável</option>
                      <option>Vegetarianas</option>
                    </select>
                  </div>
                  <div>
                    <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Tempo (min)</label>
                    <input
                      name="recipeTime"
                      type="number"
                      defaultValue={30}
                      className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                    />
                  </div>
                  <div>
                    <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Dificuldade</label>
                    <select 
                      name="recipeDifficulty" 
                      className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                    >
                      <option>Fácil</option>
                      <option>Médio</option>
                      <option>Difícil</option>
                    </select>
                  </div>
                </div>

                <div>
                  <label className="block text-xs font-bold text-stone-700 uppercase mb-1">URL da Imagem (Opcional)</label>
                  <input
                    name="recipeImage"
                    type="url"
                    placeholder="https://images.unsplash.com/..."
                    className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                  />
                </div>

                <div>
                  <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Descrição Breve</label>
                  <textarea
                    name="recipeDesc"
                    rows={2}
                    placeholder="Resumo apetitoso da sua receita..."
                    className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638]"
                  ></textarea>
                </div>

                <div>
                  <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Ingredientes (Um por linha) *</label>
                  <textarea
                    name="recipeIngredientsText"
                    rows={4}
                    required
                    placeholder="500g de Peito de Frango&#10;1 xícara de Requeijão&#10;1 colher de sal"
                    className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638] font-mono text-xs"
                  ></textarea>
                </div>

                <div>
                  <label className="block text-xs font-bold text-stone-700 uppercase mb-1">Modo de Preparo (Um passo por linha) *</label>
                  <textarea
                    name="recipeStepsText"
                    rows={4}
                    required
                    placeholder="Passo 1: Refogue o frango...&#10;Passo 2: Misture o requeijão...&#10;Passo 3: Asse por 20 minutos."
                    className="w-full px-4 py-2.5 rounded-xl border border-stone-200 text-sm outline-none focus:border-[#E05638] font-mono text-xs"
                  ></textarea>
                </div>

                <div className="pt-4 flex items-center justify-end gap-3">
                  <button
                    type="button"
                    onClick={() => setActiveTab('recipes')}
                    className="px-5 py-2.5 rounded-xl text-xs font-semibold text-stone-600 hover:bg-stone-100"
                  >
                    Cancelar
                  </button>
                  <button
                    type="submit"
                    className="bg-[#E05638] hover:bg-[#c9452a] text-white px-6 py-2.5 rounded-xl text-xs font-semibold shadow-md shadow-orange-200 transition"
                  >
                    Salvar Receita
                  </button>
                </div>
              </form>
            </div>
          </div>
        )}

      </main>

      {/* MODAL DETALHES DA RECEITA & MODO COZINHAR */}
      {selectedRecipe && (
        <div className="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm flex justify-center items-end sm:items-center p-0 sm:p-4 overflow-y-auto">
          <div className="bg-white w-full max-w-3xl rounded-t-3xl sm:rounded-3xl max-h-[90vh] overflow-y-auto shadow-2xl relative flex flex-col animate-in fade-in slide-in-from-bottom duration-300">
            
            {/* Header Image */}
            <div className="relative h-64 sm:h-72 w-full bg-stone-900">
              <img 
                src={selectedRecipe.image} 
                alt={selectedRecipe.title} 
                className="w-full h-full object-cover opacity-90"
              />
              <div className="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent"></div>

              {/* Close Button */}
              <button
                onClick={() => setSelectedRecipe(null)}
                className="absolute top-4 right-4 bg-white/80 hover:bg-white text-stone-800 p-2 rounded-full backdrop-blur-md transition shadow-md"
              >
                <X size={20} />
              </button>

              {/* Title & Info on Image */}
              <div className="absolute bottom-4 left-4 right-4 text-white space-y-1">
                <span className="bg-[#E05638] text-white text-[10px] font-bold px-2.5 py-0.5 rounded-full uppercase tracking-wider">
                  {selectedRecipe.category}
                </span>
                <h2 className="text-2xl sm:text-3xl font-extrabold">{selectedRecipe.title}</h2>
                <div className="flex flex-wrap items-center gap-4 text-xs text-stone-200 pt-1">
                  <span className="flex items-center gap-1"><Clock size={14} /> {selectedRecipe.prepTime} minutos</span>
                  <span>•</span>
                  <span className="flex items-center gap-1"><Flame size={14} /> {selectedRecipe.calories} kcal</span>
                  <span>•</span>
                  <span>Dificuldade: {selectedRecipe.difficulty}</span>
                </div>
              </div>
            </div>

            {/* Content Body */}
            <div className="p-6 space-y-6">
              
              {/* Description */}
              <p className="text-stone-600 text-sm leading-relaxed border-b border-stone-100 pb-4">
                {selectedRecipe.description}
              </p>

              {/* DYNAMIC PORTION SCALER */}
              <div className="bg-orange-50 border border-orange-200/60 rounded-2xl p-4 flex flex-col sm:flex-row items-center justify-between gap-4">
                <div className="flex items-center gap-2">
                  <Scale size={20} className="text-[#E05638]" />
                  <div>
                    <h4 className="font-bold text-stone-800 text-sm">Porcionador Inteligente</h4>
                    <p className="text-xs text-stone-500">Ajuste as porções para recalcular a quantidade de ingredientes</p>
                  </div>
                </div>

                <div className="flex items-center bg-white rounded-xl border border-stone-200 p-1">
                  {[2, 4, 6, 8].map(p => (
                    <button
                      key={p}
                      onClick={() => setScaledPortions(p)}
                      className={`px-3 py-1.5 rounded-lg text-xs font-bold transition ${
                        scaledPortions === p
                          ? 'bg-[#E05638] text-white shadow-sm'
                          : 'text-stone-600 hover:bg-stone-100'
                      }`}
                    >
                      {p} porções
                    </button>
                  ))}
                </div>
              </div>

              {/* INGREDIENTS & SHOPPING BUTTON */}
              <div className="space-y-3">
                <div className="flex items-center justify-between">
                  <h3 className="font-bold text-lg text-stone-800 flex items-center gap-2">
                    <Utensils size={18} className="text-[#E05638]" /> Ingredientes
                  </h3>
                  <button
                    onClick={() => addRecipeToShoppingList(selectedRecipe, scaledPortions)}
                    className="text-xs bg-emerald-50 text-[#2E7D32] hover:bg-emerald-100 px-3 py-1.5 rounded-xl font-semibold flex items-center gap-1 transition"
                  >
                    <Plus size={14} /> Adicionar à Lista de Compras
                  </button>
                </div>

                <ul className="grid grid-cols-1 sm:grid-cols-2 gap-2 pt-1">
                  {selectedRecipe.ingredients.map((ing, idx) => {
                    const ratio = scaledPortions / (selectedRecipe.basePortions || 4);
                    const calcAmount = typeof ing.amount === 'number' 
                      ? (ing.amount * ratio).toFixed(1).replace('.0', '')
                      : ing.amount;

                    return (
                      <li key={idx} className="bg-stone-50 rounded-xl p-3 text-xs flex items-center justify-between border border-stone-100">
                        <span className="text-stone-700 font-medium">{ing.name}</span>
                        <span className="font-bold text-[#E05638] bg-white px-2 py-0.5 rounded border border-stone-200">
                          {calcAmount} {ing.unit}
                        </span>
                      </li>
                    );
                  })}
                </ul>
              </div>

              {/* INSTRUCTIONS WITH CHECKBOXES & TIMER */}
              <div className="space-y-4 pt-4 border-t border-stone-100">
                <div className="flex items-center justify-between">
                  <h3 className="font-bold text-lg text-stone-800 flex items-center gap-2">
                    <BookOpen size={18} className="text-[#E05638]" /> Modo de Preparo (Passo a Passo)
                  </h3>

                  {/* Kitchen Timer Launcher */}
                  <div className="flex items-center gap-1 bg-stone-100 p-1 rounded-xl text-xs">
                    <span className="px-2 text-stone-500 font-medium">Timer:</span>
                    <button 
                      onClick={() => startTimer(5)}
                      className="px-2 py-1 bg-white hover:bg-stone-200 rounded text-stone-700 font-bold"
                    >
                      5m
                    </button>
                    <button 
                      onClick={() => startTimer(15)}
                      className="px-2 py-1 bg-white hover:bg-stone-200 rounded text-stone-700 font-bold"
                    >
                      15m
                    </button>
                    <button 
                      onClick={() => startTimer(30)}
                      className="px-2 py-1 bg-white hover:bg-stone-200 rounded text-stone-700 font-bold"
                    >
                      30m
                    </button>
                  </div>
                </div>

                <div className="space-y-3">
                  {selectedRecipe.instructions.map((step, idx) => {
                    const isDone = checkedSteps[idx];
                    return (
                      <div 
                        key={idx}
                        onClick={() => setCheckedSteps(prev => ({ ...prev, [idx]: !prev[idx] }))}
                        className={`p-4 rounded-2xl border transition cursor-pointer flex items-start gap-3 ${
                          isDone 
                            ? 'bg-emerald-50/50 border-emerald-200 text-stone-400 line-through' 
                            : 'bg-white border-stone-200 hover:border-orange-200 text-stone-800'
                        }`}
                      >
                        <button className="mt-0.5">
                          {isDone ? (
                            <CheckCircle2 size={20} className="text-[#2E7D32]" />
                          ) : (
                            <Circle size={20} className="text-stone-300" />
                          )}
                        </button>
                        <div className="flex-1 text-sm leading-relaxed">
                          <strong className={`block text-xs uppercase mb-0.5 ${isDone ? 'text-emerald-700' : 'text-[#E05638]'}`}>
                            Etapa {idx + 1}
                          </strong>
                          {step}
                        </div>
                      </div>
                    );
                  })}
                </div>
              </div>

            </div>

            {/* Modal Footer */}
            <div className="p-4 bg-stone-50 border-t border-stone-200 flex justify-end">
              <button
                onClick={() => setSelectedRecipe(null)}
                className="bg-stone-800 hover:bg-stone-900 text-white px-6 py-2 rounded-xl text-xs font-semibold transition"
              >
                Concluir
              </button>
            </div>

          </div>
        </div>
      )}

      {/* FOOTER */}
      <footer className="bg-white border-t border-stone-200 py-6 mt-12 text-center text-xs text-stone-400">
        <div className="max-w-6xl mx-auto px-4 flex flex-col sm:flex-row items-center justify-between gap-2">
          <div className="flex items-center gap-2">
            <ChefHat size={18} className="text-[#E05638]" />
            <span className="font-bold text-stone-700">CookIt App</span> — Seu Livro & Assistente Culinário Digital
          </div>
          <p>© {new Date().getFullYear()} CookIt. Cozinhe com facilidade e prazer.</p>
        </div>
      </footer>

    </div>
  );
}
