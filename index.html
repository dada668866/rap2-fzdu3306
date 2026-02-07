<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>酸奶单词 - 趣味背单词</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
  
  <!-- 配置Tailwind -->
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#3B82F6',
            secondary: '#10B981',
            accent: '#F59E0B',
            dark: '#1E293B',
            light: '#F8FAFC'
          },
          fontFamily: {
            sans: ['Inter', 'system-ui', 'sans-serif'],
          },
        },
      }
    }
  </script>
  
  <style type="text/tailwindcss">
    @layer utilities {
      .content-auto {
        content-visibility: auto;
      }
      .card-shadow {
        box-shadow: 0 10px 25px -5px rgba(59, 130, 246, 0.1), 0 8px 10px -6px rgba(59, 130, 246, 0.1);
      }
      .card-hover {
        transition: all 0.3s ease;
      }
      
      /* 为单词卡片添加平滑的过渡效果 */
      #word-card {
        transition: opacity 0.2s ease-in-out;
        will-change: opacity;
      }
      .card-hover:hover {
        transform: translateY(-5px);
        box-shadow: 0 20px 25px -5px rgba(59, 130, 246, 0.15), 0 8px 10px -6px rgba(59, 130, 246, 0.15);
      }
      .text-gradient {
        background-clip: text;
        -webkit-background-clip: text;
        color: transparent;
        background-image: linear-gradient(45deg, #3B82F6, #10B981);
      }
      .btn-bounce {
        transition: transform 0.2s ease;
      }
      .btn-bounce:active {
        transform: scale(0.95);
      }
      
      /* 移动端句号自动换行 */
      .mobile-break-after-period {
        /* 默认情况下不做特殊处理 */
      }
      
      /* 为桌面端和移动端都增加洗脑记忆和Rap记忆的行间距 */
      #mixed-sentence, #rap-sentence {
        line-height: 1.8; /* 增加行间距，使每行之间的间距更高一些 */
        text-align: left;
        word-wrap: break-word;
        white-space: pre-line; /* 保留换行但不保留多余空格 */
      }
      
      @media (max-width: 640px) {
        .mobile-break-after-period {
          white-space: pre-wrap;
          text-align: left; /* 确保文本左对齐 */
        }
        
        /* 在句号后添加换行 */
        .mobile-break-after-period::after {
          content: "";
        }
        
        /* 使用JavaScript处理句号后的换行，这里添加CSS辅助 */
        .mobile-break-after-period span.period-break {
          display: block;
        }
      }
      /* 确保Font Awesome图标在所有设备上正常显示 */
      .fa {
        display: inline-block !important;
        font-family: 'FontAwesome' !important;
        font-style: normal !important;
        font-weight: normal !important;
        line-height: 1 !important;
        speak: none;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        /* 确保图标大小在移动端足够清晰 */
        font-size: inherit !important;
      }
      
      /* 缩小例句、洗脑记忆和Rap记忆部分的喇叭图标 */
      h3 > button .fa-volume-up {
        font-size: 0.8em !important;
        width: 1em;
        height: 1em;
        display: flex !important;
        align-items: center;
        justify-content: center;
      }
      
      /* 设置标题前的彩色竖线 */
      .example-line {
        width: 3px;
        height: 0.9em;
        background-color: #3B82F6; /* 蓝色 */
        border-radius: 2px;
        align-self: center;
      }
      
      .memory-line {
        width: 3px;
        height: 0.9em;
        background-color: #10B981; /* 绿色 */
        border-radius: 2px;
        align-self: center;
      }
      
      .rap-line {
        width: 3px;
        height: 0.9em;
        background-color: #F59E0B; /* 黄色 */
        border-radius: 2px;
        align-self: center;
      }
      
      /* 移动端图标响应式优化 */
      @media (max-width: 640px) {
        .fa {
          font-size: 1.2em !important;
        }
        
        /* 确保标题前的图标在移动端正确显示 */
        h3 .fa {
          margin-right: 0.5rem;
          width: 1.2em;
          height: 1.2em;
          display: flex !important;
          align-items: center;
          justify-content: center;
        }
        
        /* 确保喇叭按钮在移动端足够大，易于点击 */
        button .fa-volume-up {
          font-size: 1.3em !important;
          width: 1.5em;
          height: 1.5em;
          display: flex !important;
          align-items: center;
          justify-content: center;
        }
      }
    }
  </style>
</head>
<body class="bg-gray-50 dark:bg-dark min-h-screen transition-colors duration-300">
  <!-- 顶部导航已移除 -->

  <!-- 主内容区 -->
  <main class="container mx-auto px-4 py-8 md:py-16">
    
    
    <!-- 单词卡片 -->
    <div class="max-w-3xl mx-auto">
      <div id="word-card" class="bg-white dark:bg-gray-800 rounded-2xl p-6 md:p-8 card-shadow card-hover transition-all duration-500">
        <!-- 单词和音标 -->
        <div class="mb-2 word-phonetic-container">
          <div class="word-container">
            <h2 id="word" class="text-3xl md:text-4xl font-bold text-gray-800 dark:text-white"></h2>
          </div>
          <div class="phonetic-container">
            <span id="phonetic" class="text-gray-500 dark:text-gray-400 italic mr-2"></span>
            <button onclick="speakWord()" class="text-primary hover:text-primary/80 transition-colors btn-bounce inline-block">
              <i class="fa fa-volume-up"></i>
            </button>
          </div>
        </div>
        <style>
          /* 默认桌面端样式 */
          .word-phonetic-container {
            display: flex;
            align-items: center;
            flex-wrap: wrap;
          }
          
          /* 移动端样式：将音标和喇叭图标移到单词下方 */
          @media (max-width: 767px) {
            .word-phonetic-container {
              flex-direction: column;
              align-items: flex-start;
            }
            .phonetic-container {
              margin-top: 0.5rem;
            }
          }
        </style>
        
        <!-- 单词释义 -->
        <div class="mb-6">
          <div id="part-of-speech"></div>
        </div>
        
        <!-- 例句 -->
        <div class="mb-6">
          <h3 class="text-lg font-semibold text-gray-700 dark:text-gray-200 mb-3 flex items-center">
            <span class="example-line mr-2"></span>例句
            <button onclick="speakExample()" class="text-primary hover:text-primary/80 transition-colors btn-bounce ml-2">
              <i class="fa fa-volume-up"></i>
            </button>
          </h3>
          <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl">
            <p id="example-sentence" class="text-gray-800 dark:text-gray-200 mb-2"></p>
            <p id="example-translation" class="text-gray-600 dark:text-gray-400 text-sm"></p>
          </div>
        </div>
        
        <!-- 中英文结合语句 -->
        <div class="mb-6">
          <h3 class="text-lg font-semibold text-gray-700 dark:text-gray-200 mb-3 flex items-center">
            <span class="memory-line mr-2"></span>洗脑记忆
            <button onclick="speakMixedSentence()" class="text-secondary hover:text-secondary/80 transition-colors btn-bounce ml-2">
              <i class="fa fa-volume-up"></i>
            </button>
          </h3>
          <p id="mixed-sentence" class="text-sm text-gray-800 dark:text-gray-200 bg-secondary/5 p-4 rounded-xl"></p>
        </div>
        
        <!-- Rap语句 -->
        <div>
          <h3 class="text-lg font-semibold text-gray-700 dark:text-gray-200 mb-3 flex items-center">
            <span class="rap-line mr-2"></span>Rap记忆
            <button onclick="speakRapSentence()" class="text-accent hover:text-accent/80 transition-colors btn-bounce ml-2">
              <i class="fa fa-volume-up"></i>
            </button>
          </h3>
          <p id="rap-sentence" class="text-sm mobile-break-after-period text-gray-800 dark:text-gray-200 bg-accent/5 p-4 rounded-xl"></p>
        </div>
      </div>
      
      <!-- 导航按钮 -->
      <div class="flex justify-between items-center mt-8">
        <button id="prev-btn" class="bg-white dark:bg-gray-700 text-gray-700 dark:text-gray-200 px-6 py-3 rounded-full shadow hover:shadow-md transition-all disabled:opacity-50 disabled:cursor-not-allowed btn-bounce">
          <i class="fa fa-arrow-left mr-2"></i>上一个
        </button>
        <span id="word-counter" class="text-gray-400 dark:text-gray-500">1/10</span>
        <button id="next-btn" class="bg-secondary text-white px-6 py-3 rounded-full shadow hover:shadow-md hover:bg-secondary/90 transition-all btn-bounce">
          下一个<i class="fa fa-arrow-right ml-2"></i>
        </button>
      </div>
    </div>
  </main>
  
  <!-- 信息弹窗 -->
  <div id="info-modal" class="fixed inset-0 bg-black/50 z-50 flex items-center justify-center hidden">
    <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 max-w-md w-full mx-4 transform transition-all">
      <div class="flex justify-between items-start mb-4">
        <h3 class="text-xl font-bold text-gray-800 dark:text-white">使用说明</h3>
        <button id="close-modal" class="text-gray-500 hover:text-gray-700 dark:text-gray-400 dark:hover:text-gray-200">
          <i class="fa fa-times"></i>
        </button>
      </div>
      <ul class="space-y-3 text-gray-600 dark:text-gray-300">
        <li class="flex items-start">
          <i class="fa fa-volume-up text-primary mt-1 mr-2"></i>
          <span>点击喇叭图标可以朗读单词和例句</span>
        </li>
        <li class="flex items-start">
          <i class="fa fa-arrow-left text-gray-500 mt-1 mr-2"></i>
          <i class="fa fa-arrow-right text-gray-500 mt-1 mr-2"></i>
          <span>使用箭头按钮切换单词</span>
        </li>

        <li class="flex items-start">
          <i class="fa fa-star text-accent mt-1 mr-2"></i>
          <span>通过趣味Rap语句和中英文洗脑内容帮助记忆单词</span>
        </li>
      </ul>
      <button id="got-it-btn" class="mt-6 w-full bg-primary text-white py-3 rounded-lg hover:bg-primary/90 transition-colors btn-bounce">
        明白了
      </button>
    </div>
  </div>
  <script>
    // 移动端句号自动换行功能 - 重写为更直接有效的实现
    function applyPeriodBreaks() {
      // 只针对rap-sentence元素处理，确保直接定位到需要换行的元素
      const rapElement = document.getElementById('rap-sentence');
      if (!rapElement) return;
      
      // 获取元素当前内容
      let content = rapElement.innerHTML;
      
      // 移除所有现有的br标签，避免重复添加
      content = content.replace(/<br\s*\/?>/gi, '');
      
      // 先将原始换行符\n替换为空格，避免双重换行导致行间距过大
      content = content.replace(/\n/g, ' ');
      
      if (window.innerWidth <= 640) {
        // 移动端处理：在句号和波浪号后添加br标签
        content = content.replace(/。/g, '。<br>').replace(/～/g, '～<br>');
      }
      
      // 立即应用处理后的内容
      rapElement.innerHTML = content;
    }
    
    // 优化版：确保所有单词的rap记忆内容都能正确换行
    const originalUpdateWordCard = updateWordCard;
    updateWordCard = function(isInitialLoad) {
      // 先调用原始函数
      originalUpdateWordCard.call(this, isInitialLoad);
      
      // 增加多次延迟调用，确保DOM完全更新后应用换行
      // 第一次调用（较短延迟）
      setTimeout(applyPeriodBreaks, 200);
      // 第二次调用（较长延迟，确保在所有DOM更新后）
      setTimeout(applyPeriodBreaks, 500);
    };
    
    // 页面加载完成后初始化
    window.addEventListener('DOMContentLoaded', function() {
      // 初始化页面
      updateWordCard(true);
      setupEventListeners();
      
      // 立即应用换行处理
      applyPeriodBreaks();
      // 添加延迟调用确保首次加载时内容正确
      setTimeout(applyPeriodBreaks, 300);
    });
    
    // 保留窗口大小改变时的监听
    window.addEventListener('resize', function() {
      setTimeout(applyPeriodBreaks, 100);
    });
    
    // 添加一个简单的点击事件监听器作为备用，但限制调用频率
    let lastClickTime = 0;
    const clickDelay = 500; // 500ms内只执行一次
    document.addEventListener('click', function() {
      const currentTime = new Date().getTime();
      if (currentTime - lastClickTime > clickDelay) {
        applyPeriodBreaks();
        lastClickTime = currentTime;
      }
    });
    
    // 检查是否有nextWord和prevWord函数，确保单词切换时也能触发换行
    if (typeof nextWord === 'function') {
      const originalNextWord = nextWord;
      nextWord = function() {
        originalNextWord.call(this);
        // 切换到下一个单词后应用换行
        setTimeout(applyPeriodBreaks, 300);
      };
    }
    
    if (typeof prevWord === 'function') {
      const originalPrevWord = prevWord;
      prevWord = function() {
        originalPrevWord.call(this);
        // 切换到上一个单词后应用换行
        setTimeout(applyPeriodBreaks, 300);
      };
    }
    
    // 单词数据 - 负责的导游主题
    const vocabularyList = [
      {
        word: "recommend",
        phonetic: "/ˌrekəˈmend/",
        partOfSpeech: "vt. 推荐；建议",
        example: "Can you recommend a good Italian restaurant near here?",
        exampleCn: "你能推荐一下附近好吃的意大利餐厅吗？",
        mixed: "我向每位来旅游的朋友都极力<strong class='text-secondary'>recommend</strong>这家本地人最爱的餐馆，<strong class='text-secondary'>recommend</strong>它的招牌菜和友好服务，经过多次体验我依然<strong class='text-secondary'>recommend</strong>这里为最佳选择。",
        rap: "朋友来访我<strong class='text-accent'>recommend</strong>，这家餐馆味道棒。服务贴心环境好，多次光顾仍向往。"
      },
      {
        word: "relevant",
        phonetic: "/ˈreləvənt/",
        partOfSpeech: "adj. 有关的；切题的",
        example: "Please make sure all the materials you submit are relevant to the research topic.",
        exampleCn: "请确保提交的材料都与研究主题有关。",
        mixed: "在准备报告时，我们必须筛选出<strong class='text-secondary'>relevant</strong>的数据，删除不<strong class='text-secondary'>relevant</strong>的信息，确保每个案例都<strong class='text-secondary'>relevant</strong>且能支持结论。",
        rap: "准备报告选<strong class='text-accent'>relevant</strong>，数据案例要精。信息紧扣主题走，论证有力逻辑清。"
      },
      {
        word: "reliable",
        phonetic: "/rɪˈlaɪəbl/",
        partOfSpeech: "adj. 可靠的；可信赖的",
        example: "We need a reliable supplier who can deliver materials on time.",
        exampleCn: "我们需要一个能按时交付材料的可靠的供应商。",
        mixed: "合作十余年，他始终是我们最<strong class='text-secondary'>reliable</strong>的合作伙伴，提供<strong class='text-secondary'>reliable</strong>的产品质量与<strong class='text-secondary'>reliable</strong>的售后服务。",
        rap: "十余年合作真<strong class='text-accent'>reliable</strong>，产品质量够硬。服务准时又周到，信任基石永固定。"
      },
      {
        word: "remarkable",
        phonetic: "/rɪˈmɑːkəbl/",
        partOfSpeech: "adj. 非凡的；显著的",
        example: "The team made remarkable progress in the final phase of the experiment.",
        exampleCn: "团队在实验最后阶段取得了显著的进展。",
        mixed: "这位年轻艺术家以<strong class='text-secondary'>remarkable</strong>的创造力完成了作品，其<strong class='text-secondary'>remarkable</strong>的细节处理赢得了<strong class='text-secondary'>remarkable</strong>的评价。",
        rap: "年轻艺术家真<strong class='text-accent'>remarkable</strong>，创意非凡细节妙。作品一出获盛赞，艺坛新星光闪耀。"
      },
      {
        word: "reserve",
        phonetic: "/rɪˈzɜːv/",
        partOfSpeech: "vt. 预订；保留 n. 储备",
        example: "I'd like to reserve a conference room for next Monday morning.",
        exampleCn: "我想为下周一上午预订一间会议室。",
        mixed: "为确保行程顺利，我提前<strong class='text-secondary'>reserve</strong>了机票和酒店，还<strong class='text-secondary'>reserve</strong>了一笔资金作为应急<strong class='text-secondary'>reserve</strong>。",
        rap: "提前<strong class='text-accent'>reserve</strong>机票酒店，资金储备也留足。行程安排妥当当，旅途无忧心满足。"
      },
      {
        word: "resolve",
        phonetic: "/rɪˈzɒlv/",
        partOfSpeech: "vt. 解决；决心 n. 决心",
        example: "The two parties finally resolved their disagreement through negotiation.",
        exampleCn: "双方最终通过谈判解决了分歧。",
        mixed: "面对技术难题，团队展现出坚定的<strong class='text-secondary'>resolve</strong>，成功<strong class='text-secondary'>resolve</strong>了核心障碍，这种<strong class='text-secondary'>resolve</strong>是项目成功的关键。",
        rap: "团队坚定有<strong class='text-accent'>resolve</strong>，难题攻关不退缩。核心障碍被清除，项目成功结硕果。"
      },
      {
        word: "respect",
        phonetic: "/rɪˈspekt/",
        partOfSpeech: "vt. 尊敬；尊重 n. 尊敬",
        example: "We should respect different cultural backgrounds and opinions.",
        exampleCn: "我们应当尊重不同的文化背景和观点。",
        mixed: "他以其专业能力赢得广泛<strong class='text-secondary'>respect</strong>，始终<strong class='text-secondary'>respect</strong>每位同事的意见，这种相互<strong class='text-secondary'>respect</strong>营造了良好氛围。",
        rap: "专业能力赢<strong class='text-accent'>respect</strong>，听取意见态度诚。相互尊重氛围好，团队协作力千钧。"
      },
      {
        word: "responsible",
        phonetic: "/rɪˈspɒnsəbl/",
        partOfSpeech: "adj. 负责的；有责任的",
        example: "Parents are responsible for creating a safe environment for their children.",
        exampleCn: "父母有责任为孩子创造安全的环境。",
        mixed: "作为一名<strong class='text-secondary'>responsible</strong>的项目经理，他对每个环节都<strong class='text-secondary'>responsible</strong>，这种<strong class='text-secondary'>responsible</strong>的态度确保了项目质量。",
        rap: "项目经理真<strong class='text-accent'>responsible</strong>，环节把控要求严。负责态度质量保，客户满意笑开颜。"
      },
      {
        word: "secure",
        phonetic: "/sɪˈkjʊə(r)/",
        partOfSpeech: "adj. 安全的；可靠的 vt. 使安全",
        example: "We need to find a secure place to store the important documents.",
        exampleCn: "我们需要找一个安全的地方存放重要文件。",
        mixed: "公司投入大量资源构建<strong class='text-secondary'>secure</strong>的网络环境，<strong class='text-secondary'>secure</strong>的数据加密系统，并<strong class='text-secondary'>secure</strong>了关键基础设施。",
        rap: "投入资源建<strong class='text-accent'>secure</strong>，网络数据双加密。关键设施稳如山，信息安全无担忧。"
      },
      {
        word: "sensitive",
        phonetic: "/ˈsensətɪv/",
        partOfSpeech: "adj. 敏感的；灵敏的",
        example: "This is a sensitive issue that requires careful handling.",
        exampleCn: "这是个需要谨慎处理的敏感的问题。",
        mixed: "在讨论这个<strong class='text-secondary'>sensitive</strong>话题时，他表现出<strong class='text-secondary'>sensitive</strong>的洞察力，并采取了<strong class='text-secondary'>sensitive</strong>的沟通方式。",
        rap: "讨论话题需<strong class='text-accent'>sensitive</strong>，洞察力强沟通巧。方式得当矛盾解，关系和谐共同好。"
      }
    ];
    
    // 当前单词索引
    let currentIndex = 0;
    
    // DOM元素
    const wordElement = document.getElementById('word');
    const phoneticElement = document.getElementById('phonetic');
    const partOfSpeechElement = document.getElementById('part-of-speech');
    const exampleElement = document.getElementById('example-sentence');
    const mixedElement = document.getElementById('mixed-sentence');
    const rapElement = document.getElementById('rap-sentence');
    const counterElement = document.getElementById('word-counter');
    const prevBtn = document.getElementById('prev-btn');
    const nextBtn = document.getElementById('next-btn');
    const infoBtn = document.getElementById('info-btn');
    const infoModal = document.getElementById('info-modal');
    const closeModal = document.getElementById('close-modal');
    const gotItBtn = document.getElementById('got-it-btn');
    const wordCard = document.getElementById('word-card');
    
    // 初始化逻辑已移至DOMContentLoaded事件监听器
    
    /* 更新单词卡片内容 - 优化版，减少闪烁 */
    function updateWordCard(isInitialLoad = false) {
      const wordData = vocabularyList[currentIndex];
      
      // 为了减少闪烁，我们不使用完全透明，而是使用更平滑的过渡效果
      if (!isInitialLoad) {
        // 只使用透明度变化，避免缩放带来的抖动，使用更短的过渡时间
        wordCard.classList.add('transition-opacity', 'duration-200', 'opacity-80');
      }
      
      // 不使用setTimeout延迟更新内容，这样可以减少闪烁
      wordElement.textContent = wordData.word;
      phoneticElement.textContent = wordData.phonetic;
      // 将每个词性行包装在单独的span标签中，并为每个span添加圆角样式
      const partsOfSpeech = wordData.partOfSpeech.split('\n').filter(part => part.trim());
      partOfSpeechElement.innerHTML = partsOfSpeech.map(part => 
        `<span class="inline-block bg-primary/10 text-primary px-3 py-1 rounded-full text-sm font-medium mb-1">${part}</span>`
      ).join('');
      exampleElement.textContent = wordData.example;
      // 更新例句中文翻译，移除括号
      const exampleTranslation = document.getElementById('example-translation');
      exampleTranslation.textContent = wordData.exampleCn.replace(/[()]/g, '');
      mixedElement.innerHTML = wordData.mixed;
      rapElement.innerHTML = wordData.rap;
      counterElement.textContent = `${currentIndex + 1}/${vocabularyList.length}`;
      
      // 更新按钮状态
      prevBtn.disabled = currentIndex === 0;
      
      // 检查是否是最后一个单词
      if (currentIndex === vocabularyList.length - 1) {
        nextBtn.innerHTML = '返回<i class="fa fa-arrow-right ml-2"></i>';
      } else {
        nextBtn.innerHTML = '下一个<i class="fa fa-arrow-right ml-2"></i>';
      }
      
      // 使用setTimeout来移除动画类，创建平滑的过渡效果
      if (!isInitialLoad) {
        setTimeout(() => {
          wordCard.classList.remove('opacity-70');
        }, 50); // 较短的延迟，让过渡更自然
      }
    }
    
    // 朗读单词
    function speakWord() {
      const word = vocabularyList[currentIndex].word;
      speakText(word);
    }
    
    // 朗读例句
    function speakExample() {
      const example = vocabularyList[currentIndex].example;
      speakText(example);
    }
    
    // 朗读洗脑记忆内容
    function speakMixedSentence() {
      const mixedSentence = document.getElementById('mixed-sentence').innerText;
      // 优化中文语音效果，使用更好的参数配置
      speakText(mixedSentence, 'zh-CN', true);
    }
    
    // 朗读Rap记忆内容
    function speakRapSentence() {
      const rapSentence = document.getElementById('rap-sentence').innerText;
      // 优化中文语音效果，使用更好的参数配置
      speakText(rapSentence, 'zh-CN', true);
    }
    
    // 文本朗读功能 - 增强版
    function speakText(text, lang = 'en-US', optimizeVoice = false) {
      // 停止任何正在进行的朗读
      window.speechSynthesis.cancel();
      
      // 创建新的语音实例
      const utterance = new SpeechSynthesisUtterance(text);
      utterance.lang = lang;
      utterance.rate = 0.9; // 稍微放慢速度
      
      // 针对中文语音进行优化
      if (lang === 'zh-CN' && optimizeVoice) {
        // 尝试选择更好的语音合成器
        const voices = window.speechSynthesis.getVoices();
        // 优先选择带有'Google'、'Microsoft'等高质量语音
        const preferredVoices = voices.filter(voice => 
          (voice.lang === 'zh-CN' || voice.lang.startsWith('zh-')) &&
          (voice.name.includes('Google') || voice.name.includes('Microsoft') || 
           voice.name.includes('Ivy') || voice.name.includes('Zira') || 
           voice.localService === false) // 通常云服务的语音质量更好
        );
        
        if (preferredVoices.length > 0) {
          utterance.voice = preferredVoices[0];
        }
        
        // 调整语音参数以获得更自然的效果
        utterance.pitch = 1.0; // 略微提升音调，使声音更活泼
        utterance.volume = 1.0; // 确保音量适中
        utterance.rate = 0.95; // 稍微调整语速，使中文朗读更自然
      }
      
      // 播放语音
      window.speechSynthesis.speak(utterance);
    }
    
    // 预加载可用的语音列表
    // 在页面加载时调用一次，确保在需要时可以获取到完整的语音列表
    document.addEventListener('DOMContentLoaded', function() {
      // 触发语音列表加载
      window.speechSynthesis.getVoices();
    });
    
    // 切换到上一个单词
    function prevWord() {
      if (currentIndex > 0) {
        currentIndex--;
        updateWordCard(false); // 传入false表示是切换单词，添加动画效果
      }
    }
    
    // 切换到下一个单词或返回第一个单词
    function nextWord() {
      if (currentIndex < vocabularyList.length - 1) {
        currentIndex++;
      } else {
        // 如果是最后一个单词，返回第一个
        currentIndex = 0;
      }
      updateWordCard(false); // 传入false表示是切换单词，添加动画效果
    }
    
    // 显示信息弹窗
    function showInfoModal() {
      infoModal.classList.remove('hidden');
      // 添加动画效果
      const modalContent = infoModal.querySelector('div');
      modalContent.classList.add('scale-95', 'opacity-0');
      setTimeout(() => {
        modalContent.classList.remove('scale-95', 'opacity-0');
        modalContent.classList.add('scale-100', 'opacity-100', 'transition-all', 'duration-300');
      }, 10);
    }
    
    // 隐藏信息弹窗
    function hideInfoModal() {
      const modalContent = infoModal.querySelector('div');
      modalContent.classList.remove('scale-100', 'opacity-100');
      modalContent.classList.add('scale-95', 'opacity-0', 'transition-all', 'duration-300');
      
      setTimeout(() => {
        infoModal.classList.add('hidden');
      }, 300);
    }
    
    // 设置事件监听器
    function setupEventListeners() {
      prevBtn.addEventListener('click', prevWord);
      nextBtn.addEventListener('click', nextWord);
      infoBtn.addEventListener('click', showInfoModal);
      closeModal.addEventListener('click', hideInfoModal);
      gotItBtn.addEventListener('click', hideInfoModal);
      
      // 键盘导航
      document.addEventListener('keydown', (e) => {
        if (e.key === 'ArrowLeft') prevWord();
        if (e.key === 'ArrowRight') nextWord();
      });
    }
    
    // 初始化应用
    document.addEventListener('DOMContentLoaded', init);
  </script>
</body>
</html>
