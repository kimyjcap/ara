# ara
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ara-bio - 100% 자연의 순수함</title>
<script src="https://cdn.tailwindcss.com"></script>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Noto+Sans+KR:wght@300;400;500;700&display=swap" rel="stylesheet">
<link href="https://cdn.jsdelivr.net/npm/remixicon@4.5.0/fonts/remixicon.css" rel="stylesheet">
<script>
tailwind.config = {
theme: {
extend: {
colors: {
primary: '#8B9D83',
secondary: '#E5E0D8'
},
borderRadius: {
'none': '0px',
'sm': '4px',
DEFAULT: '8px',
'md': '12px',
'lg': '16px',
'xl': '20px',
'2xl': '24px',
'3xl': '32px',
'full': '9999px',
'button': '8px'
}
}
}
}
</script>
<style>
:where([class^="ri-"])::before { content: "\f3c2"; }
body { font-family: 'Noto Sans KR', sans-serif; }
.product-card:hover .add-to-cart { opacity: 1; }
.product-card .add-to-cart { opacity: 0; transition: opacity 0.3s ease; }
</style>
</head>
<body class="bg-white">
<header class="fixed w-full bg-white/90 backdrop-blur-sm z-50">
<div class="container mx-auto px-6 py-4">
<div class="flex items-center justify-between">
<nav class="hidden md:flex items-center space-x-8">
<a href="#products" class="text-gray-700 hover:text-primary">제품</a>
<a href="#story" class="text-gray-700 hover:text-primary">스토리</a>
<a href="#ingredients" class="text-gray-700 hover:text-primary">성분</a>
<a href="#reviews" class="text-gray-700 hover:text-primary">리뷰</a>
</nav>
<a href="/" class="font-['Pacifico'] text-3xl text-primary">ara-bio</a>
<div class="flex items-center space-x-6">
<button class="w-10 h-10 flex items-center justify-center">
<i class="ri-search-line text-xl text-gray-700"></i>
</button>
<button class="w-10 h-10 flex items-center justify-center relative" id="cartBtn">
<i class="ri-shopping-cart-line text-xl text-gray-700"></i>
<span class="absolute -top-1 -right-1 bg-primary text-white text-xs rounded-full w-5 h-5 flex items-center justify-center">0</span>
</button>
</div>
</div>
</div>
</header>
<main>
<section class="relative h-screen">
<div class="slider h-full">
<div class="slide relative h-full" style="background-image: url('https://public.readdy.ai/ai/img_res/701bd4c2547b28dee1faf04dda086db4.jpg'); background-size: cover; background-position: center;">
<div class="absolute inset-0 bg-black/20"></div>
<div class="container mx-auto px-6 relative h-full flex items-center">
<div class="max-w-2xl text-white">
<h1 class="text-5xl font-light mb-6">자연의 순수함을 담은<br>프리미엄 영양제</h1>
<p class="text-xl mb-8">100% 천연 원료로 만든 ara-bio의 제품으로<br>건강한 라이프스타일을 시작하세요.</p>
<a href="#products" class="inline-block bg-primary text-white px-8 py-4 !rounded-button hover:bg-primary/90 transition-colors">제품 보기</a>
</div>
</div>
</div>
<div class="slide relative h-full" style="background-image: url('https://public.readdy.ai/ai/img_res/a419ccf54488c2c00fb9420367694e43.jpg'); background-size: cover; background-position: center;">
<div class="absolute inset-0 bg-black/20"></div>
<div class="container mx-auto px-6 relative h-full flex items-center">
<div class="max-w-2xl text-white">
<h1 class="text-5xl font-light mb-6">순수한 자연의 힘</h1>
<p class="text-xl mb-8">엄선된 원료만을 사용하여<br>건강한 삶을 선사합니다.</p>
<a href="#products" class="inline-block bg-primary text-white px-8 py-4 !rounded-button hover:bg-primary/90 transition-colors">제품 보기</a>
</div>
</div>
</div>
<div class="slide relative h-full" style="background-image: url('https://public.readdy.ai/ai/img_res/c97f1bf4ea3cbc6bbc45f0b02af8674d.jpg'); background-size: cover; background-position: center;">
<div class="absolute inset-0 bg-black/20"></div>
<div class="container mx-auto px-6 relative h-full flex items-center">
<div class="max-w-2xl text-white">
<h1 class="text-5xl font-light mb-6">과학으로 증명된<br>자연의 효능</h1>
<p class="text-xl mb-8">현대 과학과 자연의 조화로<br>더 나은 건강을 약속합니다.</p>
<a href="#products" class="inline-block bg-primary text-white px-8 py-4 !rounded-button hover:bg-primary/90 transition-colors">제품 보기</a>
</div>
</div>
</div>
<button class="absolute left-4 top-1/2 -translate-y-1/2 w-12 h-12 flex items-center justify-center bg-white/30 hover:bg-white/50 rounded-full text-white z-10" onclick="prevSlide()">
<i class="ri-arrow-left-s-line text-2xl"></i>
</button>
<button class="absolute right-4 top-1/2 -translate-y-1/2 w-12 h-12 flex items-center justify-center bg-white/30 hover:bg-white/50 rounded-full text-white z-10" onclick="nextSlide()">
<i class="ri-arrow-right-s-line text-2xl"></i>
</button>
<div class="absolute bottom-8 left-1/2 -translate-x-1/2 flex space-x-2 z-10">
<button class="w-2 h-2 rounded-full bg-white/50 dot active"></button>
<button class="w-2 h-2 rounded-full bg-white/50 dot"></button>
<button class="w-2 h-2 rounded-full bg-white/50 dot"></button>
</div>
</div>
</section>
<section id="products" class="py-24 bg-gray-50">
<div class="container mx-auto px-6">
<h2 class="text-3xl text-center mb-16">베스트셀러 제품</h2>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
<div class="product-card bg-white rounded-lg overflow-hidden shadow-sm hover:shadow-md transition-shadow">
<img src="https://public.readdy.ai/ai/img_res/4fdaee30b7ed9b8601d945c4c1a48296.jpg" alt="레몬버베나" class="w-full h-64 object-cover">
<div class="p-6">
<h3 class="text-xl mb-2">레몬버베나 슬로컷</h3>
<p class="text-gray-600 mb-4">천연 레몬버베나의 진정한 향</p>
<div class="flex items-center justify-between">
<span class="text-lg">₩65,000</span>
<button class="add-to-cart bg-primary text-white px-4 py-2 !rounded-button hover:bg-primary/90 transition-colors whitespace-nowrap">장바구니 담기</button>
</div>
</div>
</div>
<div class="product-card bg-white rounded-lg overflow-hidden shadow-sm hover:shadow-md transition-shadow relative">
<div class="absolute inset-0 bg-black/60 flex items-center justify-center">
<span class="text-white text-xl font-medium">Coming Soon</span>
</div>
<img src="https://public.readdy.ai/ai/img_res/5befb25c9bdbf5a8435378e513373c85.jpg" alt="출시예정" class="w-full h-64 object-cover">
<div class="p-6">
<h3 class="text-xl mb-2">신제품 출시예정</h3>
<p class="text-gray-600 mb-4">곧 만나보실 수 있습니다</p>
<div class="flex items-center justify-between">
<span class="text-lg">-</span>
<button class="bg-gray-300 text-white px-4 py-2 !rounded-button cursor-not-allowed whitespace-nowrap" disabled>출시예정</button>
</div>
</div>
</div>
<div class="product-card bg-white rounded-lg overflow-hidden shadow-sm hover:shadow-md transition-shadow relative">
<div class="absolute inset-0 bg-black/60 flex items-center justify-center">
<span class="text-white text-xl font-medium">Coming Soon</span>
</div>
<img src="https://public.readdy.ai/ai/img_res/d7473bec48a2c643fbce478da853af32.jpg" alt="출시예정" class="w-full h-64 object-cover">
<div class="p-6">
<h3 class="text-xl mb-2">신제품 출시예정</h3>
<p class="text-gray-600 mb-4">곧 만나보실 수 있습니다</p>
<div class="flex items-center justify-between">
<span class="text-lg">-</span>
<button class="bg-gray-300 text-white px-4 py-2 !rounded-button cursor-not-allowed whitespace-nowrap" disabled>출시예정</button>
</div>
</div>
</div>
</div>
</div>
</section>
<section id="story" class="py-24">
<div class="container mx-auto px-6">
<div class="flex flex-col md:flex-row items-center gap-12">
<div class="w-full md:w-1/2">
<img src="https://public.readdy.ai/ai/img_res/40537ebb80f3b19d8d99cef8b8e9569e.jpg" alt="브랜드 스토리" class="rounded-lg w-full">
</div>
<div class="w-full md:w-1/2">
<h2 class="text-3xl mb-6">자연과 과학의 조화</h2>
<p class="text-gray-600 mb-4">ara-bio는 자연의 순수한 성분과 현대 과학의 정밀함을 결합하여 최고 품질의 영양제를 만듭니다.</p>
<p class="text-gray-600 mb-8">모든 제품은 엄격한 품질 관리 하에 생산되며, 천연 원료만을 사용하여 건강과 환경을 모두 생각합니다.</p>
<a href="#about" class="inline-block bg-primary text-white px-6 py-3 !rounded-button hover:bg-primary/90 transition-colors">더 알아보기</a>
</div>
</div>
</div>
</section>
<section id="about" class="py-24 bg-white">
<div class="container mx-auto px-6">
<div class="max-w-4xl mx-auto">
<h2 class="text-4xl text-center mb-16">우리의 이념</h2>
<div class="space-y-16">
<div class="flex flex-col md:flex-row items-center gap-12">
<div class="w-full md:w-1/2">
<img src="https://public.readdy.ai/ai/img_res/0b13422aac763d2aea75ef9e6a8a3338.jpg" alt="자연의 순수함" class="rounded-lg w-full">
</div>
<div class="w-full md:w-1/2">
<h3 class="text-2xl mb-4">자연의 순수함</h3>
<p class="text-gray-600">ara-bio는 자연의 순수한 힘을 믿습니다. 우리는 전 세계에서 가장 순수한 원료만을 선별하여 사용합니다. 각 원료는 그 고유의 효능을 최대한 보존하면서도, 현대인의 건강에 최적화된 형태로 제공됩니다.</p>
</div>
</div>
<div class="flex flex-col md:flex-row items-center gap-12">
<div class="w-full md:w-1/2 order-2 md:order-1">
<h3 class="text-2xl mb-4">과학적 혁신</h3>
<p class="text-gray-600">최첨단 연구 시설과 전문 연구진을 통해 자연 원료의 효능을 과학적으로 입증하고 개발합니다. 우리의 모든 제품은 수년간의 연구와 임상시험을 거쳐 그 안전성과 효과가 검증되었습니다.</p>
</div>
<div class="w-full md:w-1/2 order-1 md:order-2">
<img src="https://public.readdy.ai/ai/img_res/c23f066f41f24c3a12d6f41ad04662d5.jpg" alt="과학적 혁신" class="rounded-lg w-full">
</div>
</div>
<div class="flex flex-col md:flex-row items-center gap-12">
<div class="w-full md:w-1/2">
<img src="https://public.readdy.ai/ai/img_res/35d2bff90d9c945f4c2ee1306eec6a28.jpg" alt="지속가능성" class="rounded-lg w-full">
</div>
<div class="w-full md:w-1/2">
<h3 class="text-2xl mb-4">지속가능성</h3>
<p class="text-gray-600">환경 보호는 우리의 핵심 가치입니다. 생산 과정에서 발생하는 환경 영향을 최소화하고, 재생 가능한 에너지를 사용하며, 재활용 가능한 포장재만을 사용합니다. 우리는 지구와 인류의 건강한 미래를 위해 노력합니다.</p>
</div>
</div>
<div class="flex flex-col md:flex-row items-center gap-12">
<div class="w-full md:w-1/2 order-2 md:order-1">
<h3 class="text-2xl mb-4">품질 보증</h3>
<p class="text-gray-600">ara-bio의 모든 제품은 국제 GMP 기준을 준수하며, 원료 선정부터 최종 제품까지 엄격한 품질 관리 시스템을 통과합니다. 우리는 고객에게 최고 품질의 제품만을 제공하기 위해 끊임없이 노력합니다.</p>
</div>
<div class="w-full md:w-1/2 order-1 md:order-2">
<img src="https://public.readdy.ai/ai/img_res/babde872f63ae0d064b95ea2b2a13295.jpg" alt="품질 보증" class="rounded-lg w-full">
</div>
</div>
</div>
</div>
</div>
</section>
<section id="ingredients" class="py-24 bg-secondary/20">
<div class="container mx-auto px-6">
<h2 class="text-3xl text-center mb-16">엄선된 원료</h2>
<div class="grid grid-cols-1 md:grid-cols-2 gap-12 mb-16">
<div>
<img src="https://public.readdy.ai/ai/img_res/ffe1d59d92aa62acd8568a3bb8a6ff56.jpg" alt="원료 검수" class="rounded-lg w-full h-80 object-cover mb-8">
<div class="grid grid-cols-2 gap-8">
<div class="text-center">
<div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
<i class="ri-leaf-line text-3xl text-primary"></i>
</div>
<h3 class="text-xl mb-2">100% 천연 원료</h3>
<p class="text-gray-600">화학 첨가물 없이 순수한 자연 성분만 사용</p>
</div>
<div class="text-center">
<div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
<i class="ri-test-tube-line text-3xl text-primary"></i>
</div>
<h3 class="text-xl mb-2">과학적 검증</h3>
<p class="text-gray-600">철저한 연구와 임상시험을 거친 원료 선정</p>
</div>
</div>
</div>
<div>
<img src="https://public.readdy.ai/ai/img_res/20096c1ff89a4a8a5685bb2acaecdf5f.jpg" alt="생산 시설" class="rounded-lg w-full h-80 object-cover mb-8">
<div class="grid grid-cols-2 gap-8">
<div class="text-center">
<div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
<i class="ri-shield-check-line text-3xl text-primary"></i>
</div>
<h3 class="text-xl mb-2">안전성 보장</h3>
<p class="text-gray-600">국제 기준을 충족하는 품질 관리</p>
</div>
<div class="text-center">
<div class="w-16 h-16 mx-auto mb-4 flex items-center justify-center">
<i class="ri-recycle-line text-3xl text-primary"></i>
</div>
<h3 class="text-xl mb-2">친환경 생산</h3>
<p class="text-gray-600">지속 가능한 방식으로 생산 및 포장</p>
</div>
</div>
</div>
</div>
</div>
</section>
<section id="reviews" class="py-24">
<div class="container mx-auto px-6">
<h2 class="text-3xl text-center mb-16">실시간 고객 후기</h2>
<div class="relative overflow-hidden" style="height: 480px;">
<div id="reviewsContainer" class="absolute w-full transition-transform duration-500">
<div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-8">
<div class="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
<div class="flex items-center mb-4">
<img src="https://public.readdy.ai/ai/img_res/592b14de679db7ec50cae763dabdcc27.jpg" class="w-12 h-12 rounded-full object-cover mr-4" alt="프로필">
<div>
<p class="font-medium">김서연</p>
<div class="flex text-primary">
<i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i>
<span class="ml-2 text-gray-600">5.0</span>
</div>
</div>
</div>
<p class="text-gray-600 mb-4">"매일 복용하면서 확실히 컨디션이 좋아진 것을 느낍니다. 특히 피로감이 줄어들었어요. 자연스러운 원료로 만들어져서 더욱 신뢰가 갑니다."</p>
<p class="text-sm text-gray-400">2025.02.23</p>
</div>
<div class="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
<div class="flex items-center mb-4">
<img src="https://public.readdy.ai/ai/img_res/caf0283cea3c8a3786818aecf093a8ab.jpg" class="w-12 h-12 rounded-full object-cover mr-4" alt="프로필">
<div>
<p class="font-medium">이준호</p>
<div class="flex text-primary">
<i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i>
<span class="ml-2 text-gray-600">5.0</span>
</div>
</div>
</div>
<p class="text-gray-600 mb-4">"천연 원료만 사용한다는 점이 마음에 들어요. 안심하고 먹을 수 있어서 좋습니다. 포장도 환경을 생각한 것 같아 더욱 만족스럽습니다."</p>
<p class="text-sm text-gray-400">2025.02.22</p>
</div>
<div class="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
<div class="flex items-center mb-4">
<img src="https://public.readdy.ai/ai/img_res/e0da5ed881a92ffb00cb7862952d3210.jpg" class="w-12 h-12 rounded-full object-cover mr-4" alt="프로필">
<div>
<p class="font-medium">박지현</p>
<div class="flex text-primary">
<i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-half-fill"></i>
<span class="ml-2 text-gray-600">4.5</span>
</div>
</div>
</div>
<p class="text-gray-600 mb-4">"프로바이오틱스 제품이 특히 좋았어요. 장 건강이 눈에 띄게 개선되었습니다. 꾸준히 섭취하고 있어요."</p>
<p class="text-sm text-gray-400">2025.02.21</p>
</div>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-8">
<div class="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
<div class="flex items-center mb-4">
<img src="https://public.readdy.ai/ai/img_res/f8fb114c6ea9f14fcea95a5b00c6a2cf.jpg" class="w-12 h-12 rounded-full object-cover mr-4" alt="프로필">
<div>
<p class="font-medium">최미영</p>
<div class="flex text-primary">
<i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i>
<span class="ml-2 text-gray-600">5.0</span>
</div>
</div>
</div>
<p class="text-gray-600 mb-4">"3개월째 복용 중인데 피부 컨디션이 눈에 띄게 좋아졌어요. 무엇보다 성분이 믿을 수 있어서 좋습니다."</p>
<p class="text-sm text-gray-400">2025.02.20</p>
</div>
<div class="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
<div class="flex items-center mb-4">
<img src="https://public.readdy.ai/ai/img_res/50e51b31f1eee61d252f29cc74ca33b3.jpg" class="w-12 h-12 rounded-full object-cover mr-4" alt="프로필">
<div>
<p class="font-medium">강동현</p>
<div class="flex text-primary">
<i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i>
<span class="ml-2 text-gray-600">5.0</span>
</div>
</div>
</div>
<p class="text-gray-600 mb-4">"직장인이라 피로감이 심했는데, 이 제품 덕분에 활력이 많이 생겼어요. 동료들에게도 추천했습니다."</p>
<p class="text-sm text-gray-400">2025.02.19</p>
</div>
<div class="bg-white p-6 rounded-lg shadow-sm hover:shadow-md transition-shadow">
<div class="flex items-center mb-4">
<img src="https://public.readdy.ai/ai/img_res/fd3deff65189ba4c6e5e029ee2b0225a.jpg" class="w-12 h-12 rounded-full object-cover mr-4" alt="프로필">
<div>
<p class="font-medium">정유진</p>
<div class="flex text-primary">
<i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i><i class="ri-star-fill"></i>
<span class="ml-2 text-gray-600">5.0</span>
</div>
</div>
</div>
<p class="text-gray-600 mb-4">"친구 추천으로 시작했는데 정말 만족스러워요. 특히 아침에 일어날 때 개운함이 달라졌어요."</p>
<p class="text-sm text-gray-400">2025.02.18</p>
</div>
</div>
</div>
</div>
</div>
</section>
<script>
const reviewsContainer = document.getElementById('reviewsContainer');
let currentReviewPosition = 0;
function moveReviews() {
  const containerHeight = reviewsContainer.offsetHeight;
  const visibleHeight = 480; // 보이는 영역의 높이
  
  currentReviewPosition -= 1; // 1픽셀씩 위로 이동
  
  if (Math.abs(currentReviewPosition) >= containerHeight / 2) {
    currentReviewPosition = 0;
  }
  
  reviewsContainer.style.transform = `translateY(${currentReviewPosition}px)`;
}
setInterval(moveReviews, 50); // 50ms마다 이동
</script>
<section class="py-24 bg-primary/10">
<div class="container mx-auto px-6">
<div class="max-w-2xl mx-auto text-center">
<h2 class="text-3xl mb-6">뉴스레터 구독</h2>
<p class="text-gray-600 mb-8">건강한 라이프스타일을 위한 최신 소식과 특별한 혜택을 받아보세요.</p>
<form class="flex gap-4 max-w-md mx-auto">
<input type="email" placeholder="이메일 주소" class="flex-1 px-4 py-3 rounded-button border-none">
<button type="submit" class="bg-primary text-white px-6 py-3 !rounded-button hover:bg-primary/90 transition-colors whitespace-nowrap">구독하기</button>
</form>
</div>
</div>
</section>
</main>
<footer class="bg-gray-900 text-white py-16">
<div class="container mx-auto px-6">
<div class="grid grid-cols-1 md:grid-cols-4 gap-12">
<div>
<a href="/" class="font-['Pacifico'] text-2xl text-white mb-6 block">ara-bio</a>
<p class="text-gray-400">자연의 순수함을 담은<br>프리미엄 영양제</p>
</div>
<div>
<h3 class="text-lg font-medium mb-4">제품</h3>
<ul class="space-y-2">
<li><a href="#" class="text-gray-400 hover:text-white">레몬버베나 슬로핏</a></li>
</ul>
</div>
<div>
<h3 class="text-lg font-medium mb-4">고객지원</h3>
<ul class="space-y-2">
<li><a href="#" class="text-gray-400 hover:text-white">자주 묻는 질문</a></li>
<li><a href="#" class="text-gray-400 hover:text-white">배송 안내</a></li>
<li><a href="#" class="text-gray-400 hover:text-white">반품/교환</a></li>
<li><a href="#" class="text-gray-400 hover:text-white">고객센터</a></li>
</ul>
</div>
<div>
<h3 class="text-lg font-medium mb-4">회사 정보</h3>
<ul class="space-y-2">
<li class="text-gray-400">제주시 조천읍 남조로 3108 104-201</li>
<li class="text-gray-400">고객센터: 1544-1234</li>
<li class="text-gray-400">이메일: kimyjcap@naver.com</li>
<li class="flex space-x-4 mt-4">
<a href="#" class="text-gray-400 hover:text-white">
<i class="ri-instagram-line"></i>
</a>
<a href="#" class="text-gray-400 hover:text-white">
<i class="ri-facebook-line"></i>
</a>
<a href="#" class="text-gray-400 hover:text-white">
<i class="ri-youtube-line"></i>
</a>
</li>
</ul>
</div>
</div>
<div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
<p>&copy; 2025 ara-bio. All rights reserved.</p>
</div>
</div>
</footer>
<div id="cart" class="fixed inset-y-0 right-0 w-96 bg-white shadow-lg transform translate-x-full transition-transform duration-300 z-50">
<div class="p-6 h-full flex flex-col">
<div class="flex items-center justify-between mb-6">
<h3 class="text-xl font-medium">장바구니</h3>
<button id="closeCart" class="w-10 h-10 flex items-center justify-center">
<i class="ri-close-line text-xl"></i>
</button>
</div>
<div id="cartItems" class="flex-1 overflow-auto">
<!-- Cart items will be inserted here -->
</div>
<div class="border-t pt-4">
<div class="flex justify-between mb-4">
<span>총 금액</span>
<span id="totalPrice">₩0</span>
</div>
<button class="w-full bg-primary text-white py-3 !rounded-button hover:bg-primary/90 transition-colors">결제하기</button>
</div>
</div>
</div>
<script>
const cart = document.getElementById('cart');
const cartBtn = document.getElementById('cartBtn');
const closeCart = document.getElementById('closeCart');
const cartItems = document.getElementById('cartItems');
const totalPrice = document.getElementById('totalPrice');
let items = [];
let currentSlide = 0;
const slides = document.querySelectorAll('.slide');
const dots = document.querySelectorAll('.dot');
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
anchor.addEventListener('click', function (e) {
e.preventDefault();
const targetId = this.getAttribute('href');
const targetElement = document.querySelector(targetId);
if (targetElement) {
window.scrollTo({
top: targetElement.offsetTop - 80,
behavior: 'smooth'
});
}
});
});
function showSlide(index) {
slides.forEach((slide, i) => {
slide.style.display = i === index ? 'block' : 'none';
});
dots.forEach((dot, i) => {
dot.classList.toggle('bg-white', i === index);
dot.classList.toggle('bg-white/50', i !== index);
});
}
function nextSlide() {
currentSlide = (currentSlide + 1) % slides.length;
showSlide(currentSlide);
}
function prevSlide() {
currentSlide = (currentSlide - 1 + slides.length) % slides.length;
showSlide(currentSlide);
}
dots.forEach((dot, i) => {
dot.addEventListener('click', () => {
currentSlide = i;
showSlide(currentSlide);
});
});
setInterval(nextSlide, 8000);
showSlide(0);
cartBtn.addEventListener('click', () => {
cart.classList.remove('translate-x-full');
});
closeCart.addEventListener('click', () => {
cart.classList.add('translate-x-full');
});
document.querySelectorAll('.add-to-cart').forEach(button => {
button.addEventListener('click', (e) => {
if (button.disabled) return;
const card = e.target.closest('.product-card');
const name = card.querySelector('h3').textContent;
const price = parseInt(card.querySelector('span').textContent.replace(/[^0-9]/g, ''));
items.push({ name, price });
updateCart();
cart.classList.remove('translate-x-full');
});
});
function updateCart() {
cartItems.innerHTML = items.map(item => `
<div class="flex justify-between items-center py-3 border-b">
<div>
<h4 class="font-medium">${item.name}</h4>
<p class="text-gray-600">₩${item.price.toLocaleString()}</p>
</div>
<button class="text-red-500 hover:text-red-700">
<i class="ri-delete-bin-line"></i>
</button>
</div>
`).join('');
const total = items.reduce((sum, item) => sum + item.price, 0);
totalPrice.textContent = `₩${total.toLocaleString()}`;
document.querySelector('#cartBtn span').textContent = items.length;
}
</script>
</body>
</html>
