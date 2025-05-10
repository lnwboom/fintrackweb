<template>
    <section id="start"
        class="relative flex-1 flex items-center justify-center bg-gradient-to-br from-sky-100 via-sky-50 to-white py-32 overflow-hidden">
        <!-- Decorative elements -->
        <div class="absolute inset-0 overflow-hidden">
            <div
                class="absolute -top-40 -right-40 w-80 h-80 bg-sky-200 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob">
            </div>
            <div
                class="absolute -bottom-40 -left-40 w-80 h-80 bg-sky-100 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-2000">
            </div>
            <div
                class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-80 h-80 bg-sky-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-blob animation-delay-4000">
            </div>
        </div>

        <div class="relative text-center px-6 max-w-3xl">
            <h1 class="text-5xl md:text-6xl font-bold text-sky-900 mb-6 leading-tight">
                เริ่มจด <span
                    class="text-transparent bg-clip-text bg-gradient-to-r from-sky-400 to-sky-200">รายจ่าย</span>
                กันเลย!
            </h1>
            <p class="text-xl text-slate-600 mb-8 leading-relaxed">
                จัดการการเงินง่าย ๆ ด้วยแอป Fintrack<br>
                เริ่มต้นการออมเงินอย่างมีประสิทธิภาพวันนี้
            </p>
            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <!--  <button
                    class="w-full sm:w-auto bg-gradient-to-r from-sky-400 to-sky-300 hover:from-sky-300 hover:to-sky-200 text-white font-semibold px-8 py-4 rounded-full shadow-lg hover:shadow-xl transition-all duration-200 transform hover:-translate-y-0.5">
                    ลงชื่อเข้าใช้
                </button>
                <button
                    class="w-full sm:w-auto bg-white/80 hover:bg-white/90 text-sky-600 font-semibold px-8 py-4 rounded-full shadow-lg hover:shadow-xl transition-all duration-200 backdrop-blur-sm">
                    ดูวิดีโอแนะนำ
                </button>-->
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'HeroSection'
}
</script>

<style scoped>
.animate-blob {
    animation: blob 7s infinite;
}

.animation-delay-2000 {
    animation-delay: 2s;
}

.animation-delay-4000 {
    animation-delay: 4s;
}

@keyframes blob {
    0% {
        transform: translate(0px, 0px) scale(1);
    }

    33% {
        transform: translate(30px, -50px) scale(1.1);
    }

    66% {
        transform: translate(-20px, 20px) scale(0.9);
    }

    100% {
        transform: translate(0px, 0px) scale(1);
    }
}
</style>