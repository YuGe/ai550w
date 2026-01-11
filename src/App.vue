<script setup lang="ts">
import Button from "./components/Button.vue";
import Card from "./components/Card.vue";
</script>

<template>
  <div
    class="min-h-screen bg-gradient-to-b from-slate-950 to-slate-900 text-slate-100 relative overflow-hidden"
  >
    <!-- MOSS-like background grid -->
    <div
      class="pointer-events-none absolute inset-0 bg-[radial-gradient(circle_at_1px_1px,rgba(99,102,241,0.15)_1px,transparent_0)] [background-size:40px_40px] opacity-30"
    />

    <!-- Hero -->
    <section
      class="px-8 py-28 max-w-7xl mx-auto grid md:grid-cols-2 gap-12 items-center"
    >
      <div>
        <p class="text-indigo-400 uppercase tracking-widest mb-4">
          Clinically driven · AI-enabled · Resistance-focused
        </p>

        <h1 class="text-5xl font-bold leading-tight">
          Adaptive Intelligence for
          <span class="text-indigo-400">Drug Resistance</span>
        </h1>

        <p class="mt-6 text-lg text-slate-300">
          AI550W 是一家由真实临床未满足需求驱动的肿瘤新药研发公司，
          聚焦以铂类为代表的治疗耐药问题， 通过
          AI、生物信息学与转化医学系统性推进
          可合作、可注册的新一代耐药逆转药物。
        </p>

        <div class="mt-8 flex gap-4">
          <Button size="lg">Our Platform</Button>
          <Button size="lg" variant="outline">Partner with Us</Button>
        </div>
      </div>

      <div class="bg-slate-800/60 rounded-2xl p-8 shadow-xl">
        <div class="text-indigo-400 text-5xl font-bold mb-2">AI550W</div>
        <p class="text-slate-300 text-sm">
          Clinical Failure × Multi-Omics × AI × Translational Science
        </p>
      </div>
    </section>

    <!-- Platform -->
    <section class="px-8 py-24 max-w-7xl mx-auto">
      <h2 class="text-3xl font-semibold text-center mb-4">
        The AI550W Platform
      </h2>

      <p class="text-center text-slate-400 mb-12 max-w-4xl mx-auto">
        一个从临床失败场景出发、专为耐药问题设计的转化医学与 AI 系统，
        将复杂的耐药生物学转化为可落地的新药资产。
      </p>

      <div class="grid md:grid-cols-3 gap-8">
        <Card>
          <div class="p-6">
            <h3 class="text-xl font-semibold">Clinically Anchored Discovery</h3>
            <p class="mt-2 text-slate-300">
              从真实世界治疗失败与耐药表型出发， 整合多癌种多组学与临床数据。
            </p>
          </div>
        </Card>

        <Card>
          <div class="p-6">
            <h3 class="text-xl font-semibold">
              Resistance-Reversal Drug Design
            </h3>
            <p class="mt-2 text-slate-300">
              围绕明确的转化假设， 优先布局低毒性、联合友好的新机制药物。
            </p>
          </div>
        </Card>

        <Card>
          <div class="p-6">
            <h3 class="text-xl font-semibold">
              Translational & BD-Ready Strategy
            </h3>
            <p class="mt-2 text-slate-300">
              每一条管线天然符合跨国药企 BD 与并购评估逻辑。
            </p>
          </div>
        </Card>
      </div>
    </section>

    <!-- Footer -->
    <footer
      class="px-8 py-12 border-t border-slate-800 text-center text-slate-400"
    >
      <p class="text-xs mb-2 text-slate-500">
        A system designed to observe, model, and intervene — only when
        necessary.
      </p>
      © 2026 AI550W.com · Adaptive Intelligence for Drug Resistance · Clinically
      Driven.
    </footer>
  </div>
</template>
