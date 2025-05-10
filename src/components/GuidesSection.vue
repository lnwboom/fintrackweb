<template>
    <section id="guides" class="bg-gradient-to-b from-sky-50 to-white py-24">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-sky-900 mb-4">เริ่มต้นใช้งานง่ายๆ</h2>
                <p class="text-xl text-slate-600 max-w-2xl mx-auto">เพียงไม่กี่ขั้นตอน
                    คุณก็สามารถเริ่มต้นจัดการการเงินของคุณได้ทันที</p>
            </div>

            <div class="grid gap-12 md:grid-cols-3">
                <div v-for="(step, index) in steps" :key="step.title"
                    class="group relative bg-white/80 backdrop-blur-sm rounded-2xl p-8 transition-all duration-300 hover:bg-white/90 hover:transform hover:-translate-y-2 shadow-soft">
                    <div
                        class="absolute -top-4 -left-4 w-12 h-12 bg-gradient-to-r from-sky-400 to-sky-300 rounded-full flex items-center justify-center text-white font-bold text-xl shadow-lg">
                        {{ index + 1 }}
                    </div>
                    <div class="relative">
                        <img :src="step.image" :alt="step.title"
                            class="rounded-xl shadow-lg mb-6 w-full h-48 object-cover transform transition-transform duration-300 group-hover:scale-105" />
                        <h3 class="text-xl font-semibold text-sky-800 mb-3">{{ step.title }}</h3>
                        <p class="text-slate-600">{{ step.desc }}</p>
                    </div>
                </div>
            </div>

            <div class="text-center mt-16">
                <button
                    class="bg-gradient-to-r from-sky-400 to-sky-300 hover:from-sky-300 hover:to-sky-200 text-white font-semibold px-8 py-4 rounded-full shadow-lg hover:shadow-xl transition-all duration-200 transform hover:-translate-y-0.5">
                    เริ่มต้นใช้งานเลย
                </button>
            </div>
        </div>
    </section>
</template>

<script>
import homeImage from '/src/assets/Home.png'

export default {
    name: 'GuidesSection',
    data() {
        return {
            steps: [
                {
                    image: homeImage,
                    title: 'ดาวน์โหลดและลงชื่อเข้าใช้',
                    desc: 'ดาวน์โหลดแอป Fintrack แล้วล็อกอินด้วย Email ของคุณ'
                },
                {
                    image: homeImage,
                    title: 'ยืนยันตัวตน',
                    desc: 'กรอก Email ของคุณ แล้วรับรหัส OTP ยืนยันทาง Email เพื่อความปลอดภัย'
                },
                {
                    image: homeImage,
                    title: 'เริ่มต้นใช้งาน',
                    desc: 'ตรวจสอบข้อมูลส่วนตัวให้ถูกต้อง แล้วเริ่มต้นจัดการการเงินของคุณได้ทันที'
                }
            ]
        }
    }
}
</script>