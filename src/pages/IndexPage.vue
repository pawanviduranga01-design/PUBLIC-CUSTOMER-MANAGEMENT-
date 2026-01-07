<template>
  <q-page class="bg-white">
    <!-- Hero Section -->
    <!-- Hero Section -->
    <section
      class="q-py-xl q-px-md bg-white overflow-hidden"
      style="min-height: 90vh; display: flex; align-items: center"
    >
      <div class="container full-width" style="max-width: 1200px; margin: 0 auto">
        <div class="row items-center q-col-gutter-xl">
          <!-- Text Column -->
          <div class="col-12 col-md-6 animate-fade-up text-center text-md-left">
            <q-badge
              color="red-1"
              text-color="red"
              label="New: AI-Powered Insights"
              class="q-py-sm q-px-md text-weight-bold q-mb-lg"
              rounded
            />

            <h1
              class="text-h2 text-lg-h1 text-weight-bolder text-dark q-mb-md"
              style="line-height: 1.1"
            >
              Grow with <br />
              <span class="text-red relative-position">
                Confidence
                <svg
                  class="absolute-bottom-right"
                  width="100%"
                  height="8"
                  viewBox="0 0 100 8"
                  style="bottom: 5px; z-index: -1; opacity: 0.2"
                  preserveAspectRatio="none"
                >
                  <path d="M0 4 Q 50 8 100 4" stroke="#D50000" stroke-width="8" fill="none" />
                </svg>
              </span>
            </h1>

            <p class="text-h6 text-grey-8 q-mb-xl" style="line-height: 1.6">
              The all-in-one Customer Management System designed for modern businesses. Track,
              manage, and scale your relationships effortlessly.
            </p>

            <div class="row q-gutter-md justify-center justify-md-start">
              <q-btn
                color="primary"
                size="lg"
                icon-right="arrow_forward"
                label="Get Started Free"
                no-caps
                unelevated
                class="q-px-xl text-weight-bold shadow-10"
              />
              <q-btn
                flat
                color="dark"
                size="lg"
                icon="play_circle"
                label="Watch Demo"
                no-caps
                class="text-weight-bold"
              />
            </div>

            <div
              class="q-mt-xl text-grey-6 text-caption row items-center justify-center justify-md-start q-gutter-sm"
            >
              <q-icon name="check_circle" color="green" /> <span>No credit card required</span>
              <q-icon name="check_circle" color="green" class="q-ml-md" />
              <span>14-day free trial</span>
            </div>
          </div>

          <!-- Visual Column -->
          <div
            class="col-12 col-md-6 animate-fade-up flex flex-center"
            style="animation-delay: 0.2s"
          >
            <div class="relative-position fit">
              <!-- Decorative blob -->
              <div
                class="absolute-center bg-red-1"
                style="
                  width: 100%;
                  height: 100%;
                  border-radius: 50%;
                  filter: blur(80px);
                  opacity: 0.5;
                  z-index: 0;
                "
              ></div>

              <!-- Dashboard Image -->
              <q-img
                src="~assets/dashboard-mockup-dark.png"
                class="shadow-20 rounded-borders relative-position"
                style="z-index: 1; border: 1px solid #333"
                alt="CMS Pro Dashboard"
              />

              <!-- Floating Card -->
              <q-card
                class="absolute bg-dark text-white shadow-10 q-pa-sm animate-float"
                style="bottom: -15px; left: -15px; border-radius: 12px; z-index: 2; width: 160px"
              >
                <div class="row items-center">
                  <q-icon name="trending_up" color="green" size="sm" class="q-mr-sm" />
                  <div>
                    <div class="text-caption text-grey-5" style="font-size: 10px">Growth</div>
                    <div class="text-subtitle2 text-weight-bold">+128%</div>
                  </div>
                </div>
              </q-card>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="q-py-xl bg-white q-px-md">
      <div class="container text-center q-mb-xl">
        <h2 class="text-h3 text-weight-bold text-dark q-mb-md">Everything you need</h2>
        <p class="text-h6 text-grey-7">Powerful features to manage your customer relationships.</p>
      </div>

      <div class="row q-col-gutter-xl container q-mx-auto" style="max-width: 1200px">
        <div v-for="(feature, index) in features" :key="index" class="col-12 col-md-4">
          <q-card flat class="bg-grey-1 h-full q-pa-md hover-effect text-left">
            <q-card-section>
              <q-avatar
                :icon="feature.icon"
                color="white"
                text-color="primary"
                size="60px"
                font-size="28px"
                class="shadow-1 q-mb-md"
              />
              <div class="text-h5 text-weight-bold q-mb-sm">{{ feature.title }}</div>
              <div class="text-grey-8 text-body1">{{ feature.desc }}</div>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </section>

    <!-- Stats Section -->
    <section class="bg-dark text-white q-py-xl">
      <div class="row container q-mx-auto text-center" style="max-width: 1200px">
        <div class="col-12 col-md-4 q-mb-lg q-mb-md-none">
          <div class="text-h2 text-weight-bold text-red">10k+</div>
          <div class="text-h6 text-grey-5">Active Users</div>
        </div>
        <div class="col-12 col-md-4 q-mb-lg q-mb-md-none">
          <div class="text-h2 text-weight-bold text-red">99.9%</div>
          <div class="text-h6 text-grey-5">Uptime Guaranteed</div>
        </div>
        <div class="col-12 col-md-4">
          <div class="text-h2 text-weight-bold text-red">24/7</div>
          <div class="text-h6 text-grey-5">Expert Support</div>
        </div>
      </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" class="q-py-xl bg-grey-1 q-px-md">
      <div class="container text-center q-mb-xl">
        <h2 class="text-h3 text-weight-bold text-dark q-mb-md">Simple Pricing</h2>
        <p class="text-h6 text-grey-7">Choose the plan that fits your business needs.</p>
      </div>

      <div class="row q-col-gutter-lg container q-mx-auto justify-center" style="max-width: 1200px">
        <div v-for="(plan, index) in plans" :key="index" class="col-12 col-md-4 col-lg-3">
          <q-card
            :class="[
              'q-pa-lg',
              'text-center',
              'pricing-card',
              plan.highlight ? 'bg-dark text-white shadow-10' : 'bg-white text-dark shadow-1',
            ]"
            style="height: 100%; display: flex; flex-direction: column"
          >
            <q-card-section>
              <div class="text-uppercase text-weight-bold letter-spacing-1 q-mb-md">
                {{ plan.name }}
              </div>
              <div class="text-h2 text-weight-bold q-mb-sm">
                ${{ plan.price }}<span class="text-body1 text-weight-regular">/mo</span>
              </div>
              <div :class="plan.highlight ? 'text-grey-5' : 'text-grey-7'">{{ plan.desc }}</div>
            </q-card-section>

            <q-card-section class="q-py-lg grow">
              <q-list dense>
                <q-item
                  v-for="feature in plan.features"
                  :key="feature"
                  class="q-px-none"
                  style="min-height: 32px"
                >
                  <q-item-section avatar style="min-width: 24px">
                    <q-icon name="check" color="red" size="xs" />
                  </q-item-section>
                  <q-item-section :class="plan.highlight ? 'text-grey-4' : 'text-grey-8'">{{
                    feature
                  }}</q-item-section>
                </q-item>
              </q-list>
            </q-card-section>

            <q-card-actions align="center" class="q-mt-auto">
              <q-btn
                :color="plan.highlight ? 'red' : 'dark'"
                :outline="!plan.highlight"
                :text-color="!plan.highlight ? 'dark' : 'white'"
                unelevated
                label="Choose Plan"
                class="full-width q-py-sm text-weight-bold"
              />
            </q-card-actions>
          </q-card>
        </div>
      </div>
    </section>

    <!-- FAQ Section -->
    <section class="q-py-xl bg-white q-px-md">
      <div class="container q-mx-auto" style="max-width: 800px">
        <h2 class="text-h3 text-weight-bold text-center text-dark q-mb-xl">Common Questions</h2>

        <q-list separator>
          <q-expansion-item
            v-for="(faq, index) in faqs"
            :key="index"
            group="faqs"
            :label="faq.question"
            header-class="text-h6 text-weight-medium q-py-md"
            expand-icon-class="text-primary"
          >
            <q-card>
              <q-card-section class="text-grey-8 text-body1">
                {{ faq.answer }}
              </q-card-section>
            </q-card>
          </q-expansion-item>
        </q-list>
      </div>
    </section>

    <!-- Big CTA -->
    <section class="q-py-xl bg-red text-white text-center q-px-md">
      <div class="container q-mx-auto" style="max-width: 800px">
        <h2 class="text-h3 text-weight-bold q-mb-lg">Ready to transform your business?</h2>
        <p class="text-h5 opacity-80 q-mb-xl">Join thousands of satisfied customers today.</p>
        <q-btn
          color="white"
          text-color="red"
          size="xl"
          label="Get Started Now"
          unelevated
          no-caps
          class="text-weight-bold shadow-5"
        />
      </div>
    </section>
  </q-page>
</template>

<script setup>
const features = [
  {
    title: 'Contact Management',
    icon: 'perm_contact_calendar',
    desc: 'Centralize your customer data. View history, notes, and deals in one place.',
  },
  {
    title: 'Deal Pipeline',
    icon: 'trending_up',
    desc: 'Visualize your sales process. Drag and drop deals to move them forward.',
  },
  {
    title: 'Email Automation',
    icon: 'schedule_send',
    desc: 'Send personalized emails at scale. Follow up automatically without lifting a finger.',
  },
  {
    title: 'Analytics & Reporting',
    icon: 'insights',
    desc: 'Deep dive into your sales performance. Make data-driven decisions.',
  },
  {
    title: 'Team Collaboration',
    icon: 'groups',
    desc: 'Work together seamlessly. Assign tasks, mention colleagues, and share updates.',
  },
  {
    title: 'Mobile Access',
    icon: 'smartphone',
    desc: 'Access your CRM from anywhere. Stay connected on the go.',
  },
]

const plans = [
  {
    name: 'Starter',
    price: '0',
    desc: 'For small teams just getting started.',
    features: ['Up to 3 Users', '1,000 Contacts', 'Basic Reporting', 'Email Support'],
    highlight: false,
  },
  {
    name: 'Pro',
    price: '49',
    desc: 'Everything you need to grow.',
    features: [
      'Unlimited Users',
      '50,000 Contacts',
      'Advanced Automation',
      'Priority Support',
      'Custom Fields',
    ],
    highlight: true,
  },
  {
    name: 'Enterprise',
    price: '199',
    desc: 'For large organizations.',
    features: [
      'Unlimited Everything',
      'Dedicated Account Manager',
      'SSO & Advanced Security',
      'API Access',
      'Custom Onboarding',
    ],
    highlight: false,
  },
]

const faqs = [
  {
    question: 'Is there a free trial?',
    answer: 'Yes, we offer a 14-day free trial on all paid plans. No credit card required.',
  },
  {
    question: 'Can I import my data?',
    answer:
      'Absolutely. We support importing contacts and companies from CSV, Excel, and other major CRMs.',
  },
  {
    question: 'Is my data secure?',
    answer:
      'Security is our top priority. We use bank-grade encryption and comply with all major privacy regulations.',
  },
  {
    question: 'Can I cancel anytime?',
    answer: 'Yes, you can cancel your subscription at any time. There are no long-term contracts.',
  },
]
</script>

<style scoped>
.hover-effect {
  transition:
    transform 0.2s,
    box-shadow 0.2s;
}
.hover-effect:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}
.opacity-50 {
  opacity: 0.5;
}
.opacity-80 {
  opacity: 0.8;
}
.letter-spacing-1 {
  letter-spacing: 1px;
}

/* Pricing Card Animation */
.pricing-card {
  transition: transform 0.3s ease;
}
.pricing-card:hover {
  transform: translateY(-8px);
}

/* Animations */
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.animate-fade-up {
  animation: fadeUp 0.8s ease-out forwards;
}

/* Responsive Typography */
@media (min-width: 1024px) {
  .text-md-h1 {
    font-size: 4.5rem;
    line-height: 1.1;
  }
}
@media (max-width: 599px) {
  .text-h2 {
    font-size: 2.5rem;
  }
}

@keyframes float {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-10px);
  }
  100% {
    transform: translateY(0px);
  }
}
.animate-float {
  animation: float 4s ease-in-out infinite;
}
</style>
