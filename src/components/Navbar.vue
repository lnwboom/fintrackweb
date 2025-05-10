<template>
    <nav class="bg-white/80 backdrop-blur-sm shadow-soft sticky top-0 z-50">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <!-- logo + text -->
                <a href="/" class="flex items-center space-x-3 group">
                    <img src="/src/assets/money1.png" alt="Logo"
                        class="h-10 w-10 transition-transform group-hover:scale-110" />
                    <span
                        class="text-sky-900 font-bold text-2xl bg-gradient-to-r from-sky-400 to-sky-200 bg-clip-text text-transparent">Fintrack</span>
                </a>
                <!-- links -->
                <ul class="hidden md:flex space-x-8 text-sm font-medium">
                    <li><a href="#start"
                            class="text-slate-600 hover:text-sky-500 transition-colors duration-200">เริ่มต้นใช้งาน</a>
                    </li>
                    <li><a href="#guides"
                            class="text-slate-600 hover:text-sky-500 transition-colors duration-200">แนะนำการใช้งาน</a>
                    </li>
                    <li><a href="#features"
                            class="text-slate-600 hover:text-sky-500 transition-colors duration-200">ฟีเจอร์หลัก</a>
                    </li>
                    <li><a href="#faq"
                            class="text-slate-600 hover:text-sky-500 transition-colors duration-200">คำถามที่พบบ่อย</a>
                    </li>
                </ul>
                <!-- CTA button -->
                <button
                    class="hidden md:inline-block bg-gradient-to-r from-sky-400 to-sky-300 hover:from-sky-300 hover:to-sky-200 text-white px-6 py-2.5 rounded-lg font-medium shadow-lg hover:shadow-xl transition-all duration-200 transform hover:-translate-y-0.5">
                    ดาวน์โหลด
                </button>
                <!-- mobile menu button -->
                <button class="md:hidden text-slate-600 hover:text-sky-500 focus:outline-none">
                    <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar'
}
</script>