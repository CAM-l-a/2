<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>宏福农资 </title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#2D5A3D',
                        secondary: '#8FBC8F',
                        accent: '#FFD700',
                        neutral: '#F5F5DC',
                        dark: '#1E3A28'
                    },
                    fontFamily: {
                        sans: ['Microsoft YaHei', 'sans-serif'],
                    },
                    animation: {
                        'fade-in': 'fadeIn 2s ease-in-out',
                        'slide-up': 'slideUp 1.5s ease-out',
                        'pulse-slow': 'pulse 3s infinite',
                    },
                    keyframes: {
                        fadeIn: {
                            '0%': { opacity: '0' },
                            '100%': { opacity: '1' },
                        },
                        slideUp: {
                            '0%': { transform: 'translateY(30px)', opacity: '0' },
                            '100%': { transform: 'translateY(0)', opacity: '1' },
                        }
                    }
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .text-shadow {
                text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            }
            .bg-texture {
                background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><rect width="100" height="100" fill="%23F5F5DC" /><path d="M0,50 Q25,30 50,50 T100,50" stroke="%23E8E8D0" stroke-width="1" fill="none" /></svg>');
                background-repeat: repeat;
            }
            .highlight {
                position: relative;
                display: inline-block;
            }
            .highlight::after {
                content: '';
                position: absolute;
                bottom: -5px;
                left: 0;
                width: 100%;
                height: 3px;
                background-color: theme('colors.accent');
                transform: scaleX(0);
                transform-origin: bottom right;
                transition: transform 0.3s ease;
            }
            .highlight:hover::after {
                transform: scaleX(1);
                transform-origin: bottom left;
            }
        }
    </style>
</head>
<body class="bg-neutral bg-texture min-h-screen">
    <!-- 音频播放器（自动播放） -->
    <audio id="backgroundMusic" loop>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3" type="audio/mpeg">
    </audio>

    <!-- 页面容器 -->
    <div class="container mx-auto px-4 py-8 max-w-4xl">
        <!-- 顶部装饰 -->
        <div class="flex justify-center mb-8">
            <div class="w-16 h-2 bg-primary rounded-full mx-1 animate-pulse-slow"></div>
            <div class="w-32 h-2 bg-accent rounded-full mx-1 animate-pulse-slow" style="animation-delay: 0.5s;"></div>
            <div class="w-16 h-2 bg-primary rounded-full mx-1 animate-pulse-slow" style="animation-delay: 1s;"></div>
        </div>

        <!-- 标题部分 -->
        <header class="text-center mb-12 animate-fade-in">
            <h1 class="text-4xl md:text-5xl font-bold text-primary mb-4 text-shadow">
                <span class="highlight">宏福农资</span> 
            </h1>
            <p class="text-xl text-dark italic">同心同德 · 锐意进取 · 共创辉煌</p>
        </header>

        <!-- 主要内容 -->
        <main class="bg-white bg-opacity-90 rounded-xl shadow-lg p-6 md:p-10 mb-10 animate-slide-up">
            <div class="prose max-w-none text-dark">
                <p class="text-lg md:text-xl mb-6 leading-relaxed">
                    各位并肩前行的农资伙伴、宏福农资家人朋友们:
                </p>
                
                <p class="text-lg mb-6 leading-relaxed">
                    今天，风和日丽，月朗星稀，人间最美四月天!
                </p>
                
                <p class="text-lg mb-6 leading-relaxed">
                    今天,我们满怀喜悦与自豪，向全体家人们，致以最热烈的祝贺和最崇高的敬意!
                </p>
                
                <div class="bg-primary bg-opacity-10 border-l-4 border-primary p-4 my-8 rounded-r-lg">
                    <p class="text-lg mb-4 leading-relaxed">
                        今年，市场环境复杂多变、行业竞争日益激烈、阴雨绵绵60年一遇,我们同心同德、锐意进取,以深耕三农的初心、攻坚克难的决心、精益求精的匠心，稳扎市场、精耕服务、严控品质、拓展渠道，在产品供应、技术服务、市场占有率、客户口碑等多个维度全面突破，交出了一份逆势上扬、亮点纷呈的高质量答卷,与去年同期相比,销售总额增加<span class="text-2xl font-bold text-primary">27%以上</span>!
                    </p>
                </div>
                
                <p class="text-lg mb-6 leading-relaxed">
                    家人们，前50名的销售业绩己大幅攀升，出现了十几万、几十万的发货量。很多朋友会觉得今年生意好做了,钱赚得多了，那是你的思路对了，你长期的付出有收获了。特别是很务企业、很务经销商都快熬不下去了，你的成功尤其难得。
                </p>
                
                <div class="flex justify-center my-10">
                    <div class="w-24 h-24 rounded-full bg-accent flex items-center justify-center shadow-lg transform hover:scale-110 transition-transform duration-300">
                        <i class="fa fa-trophy text-4xl text-primary"></i>
                    </div>
                </div>
                
                <p class="text-lg mb-6 leading-relaxed">
                    当然，成绩属于过去，奋进正当其时。我们知道，没有凭空而来的成绩，只有永不言弃的坚持;没有轻而易举的突破，只有众志成城的力量。每一份订单、每一次认可、每一项业绩，都镌刻着大家的辛苦付出。愿我们携手秉持初心、乘势而上，以更昂扬的斗志、更务实的作风，深耕农资主业，守护良田沃土，再续农业辉煌!
                </p>
            </div>
        </main>

        <!-- 底部信息 -->
        <footer class="text-center text-primary animate-fade-in" style="animation-delay: 1s;">
            <div class="flex justify-center space-x-4 mb-4">
                <a href="#" class="text-primary hover:text-accent transition-colors duration-300">
                    <i class="fa fa-share-alt text-2xl"></i>
                </a>
                <a href="#" class="text-primary hover:text-accent transition-colors duration-300">
                    <i class="fa fa-thumbs-up text-2xl"></i>
                </a>
                <a href="#" class="text-primary hover:text-accent transition-colors duration-300">
                    <i class="fa fa-comment text-2xl"></i>
                </a>
            </div>
            <p class="text-sm">© 2025 宏福农资集团 | 携手共进 共创未来</p>
        </footer>
    </div>

    <!-- 控制按钮 -->
    <div class="fixed bottom-6 right-6 bg-white rounded-full shadow-lg p-3 cursor-pointer hover:bg-accent transition-colors duration-300 z-50">
        <button id="musicControl" class="text-primary hover:text-dark">
            <i class="fa fa-volume-up text-2xl"></i>
        </button>
    </div>

    <script>
        // 页面加载完成后自动播放音乐
        document.addEventListener('DOMContentLoaded', function() {
            const audio = document.getElementById('backgroundMusic');
            const musicControl = document.getElementById('musicControl');
            
            // 尝试自动播放音乐
            function playAudio() {
                audio.play().catch(error => {
                    console.log('自动播放失败，等待用户交互后播放:', error);
                    // 监听用户交互事件，一旦有交互就尝试播放
                    document.addEventListener('click', function startPlay() {
                        audio.play();
                        document.removeEventListener('click', startPlay);
                    }, { once: true });
                });
            }
            
            // 延迟一秒尝试播放，提高自动播放成功率
            setTimeout(playAudio, 1000);
            
            // 音乐控制按钮
            musicControl.addEventListener('click', function() {
                if (audio.paused) {
                    audio.play();
                    musicControl.innerHTML = '<i class="fa fa-volume-up text-2xl"></i>';
                } else {
                    audio.pause();
                    musicControl.innerHTML = '<i class="fa fa-volume-off text-2xl"></i>';
                }
            });
            
            // 添加滚动动画
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };
            
            const observer = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('animate-slide-up');
                    }
                });
            }, observerOptions);
            
            // 观察所有段落元素
            document.querySelectorAll('p').forEach(p => {
                observer.observe(p);
            });
        });
    </script>
</body>
</html>
