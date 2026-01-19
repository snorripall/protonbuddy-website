<template>
  <div class="min-h-screen bg-[#100D22] text-[#35295A]">
    <UPageHero
      title="ProtonBuddy"
      description="Automatically optimize your Linux games for maximum performance. Fine-tune launch parameters, collect performance statistics, and track improvements across kernel updates, driver changes, and game settings."
      :links="[{
        label: 'Download Now',
        to: '#download',
        trailingIcon: 'i-lucide-download',
        size: 'xl',
        color: 'primary'
      }]"
      class="bg-gradient-to-br from-[#100D22] to-[#35295A] text-white"
    />

    <UPageSection
      id="features"
      title="Key Features"
      description="Everything you need to get the best performance out of your Linux gaming setup."
      :features="[{
        icon: 'i-lucide-zap',
        title: 'Automatic Optimization',
        description: 'Automatically detect and apply optimal launch parameters for Steam games and any Linux game, tailored to your distribution, graphics card, and drivers.'
      }, {
        icon: 'i-lucide-bar-chart-3',
        title: 'Performance Tracking',
        description: 'Collect detailed statistics from game sessions to monitor performance changes over time. Track improvements from kernel updates, driver changes, or setting adjustments.'
      }, {
        icon: 'i-lucide-gamepad-2',
        title: 'Universal Compatibility',
        description: 'Works with Steam games, native Linux games, and any application. Supports various Linux distributions and graphics setups.'
      }, {
        icon: 'i-lucide-settings',
        title: 'Flexible Configuration',
        description: 'Easily customize launch options for DirectX to Vulkan conversions, shader pre-caching, and other performance tweaks.'
      }]"
      class="bg-[#0F0B1F]"
    />

    <UPageSection
      title="How It Works"
      description="Get started with ProtonBuddy in four simple steps."
      class="bg-[#100D22]"
    >
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
        <div class="text-center">
          <div class="w-16 h-16 bg-primary rounded-full flex items-center justify-center mx-auto mb-4">
            <span class="text-2xl font-bold text-white">1</span>
          </div>
          <h3 class="text-xl font-semibold mb-2 text-[#35295A]">Install ProtonBuddy</h3>
          <p class="text-gray-600">Download and install the desktop application on your Linux system.</p>
        </div>
        <div class="text-center">
          <div class="w-16 h-16 bg-primary rounded-full flex items-center justify-center mx-auto mb-4">
            <span class="text-2xl font-bold text-white">2</span>
          </div>
          <h3 class="text-xl font-semibold mb-2 text-[#35295A]">Select Your Games</h3>
          <p class="text-gray-600">Choose games from Steam or manually add any Linux executable.</p>
        </div>
        <div class="text-center">
          <div class="w-16 h-16 bg-primary rounded-full flex items-center justify-center mx-auto mb-4">
            <span class="text-2xl font-bold text-white">3</span>
          </div>
          <h3 class="text-xl font-semibold mb-2 text-[#35295A]">Let It Optimize</h3>
          <p class="text-gray-600">ProtonBuddy automatically applies optimal launch parameters based on your hardware and software configuration.</p>
        </div>
        <div class="text-center">
          <div class="w-16 h-16 bg-primary rounded-full flex items-center justify-center mx-auto mb-4">
            <span class="text-2xl font-bold text-white">4</span>
          </div>
          <h3 class="text-xl font-semibold mb-2 text-[#35295A]">Monitor Performance</h3>
          <p class="text-gray-600">View detailed statistics and performance history to see the impact of system updates and configuration changes.</p>
        </div>
      </div>
    </UPageSection>

    <UPageSection id="download" class="bg-[#0F0B1F]">
      <UPageCTA
        title="Ready to Optimize Your Gaming?"
        description="Download ProtonBuddy today and experience the best Linux gaming performance."
        :links="[{
          label: 'Download for Linux',
          to: '#',
          trailingIcon: 'i-lucide-download',
          color: 'primary',
          size: 'xl'
        }]"
      />
    </UPageSection>

    <footer class="bg-[#0A0814] py-8 text-center">
      <p class="text-gray-600">&copy; 2024 ProtonBuddy. Built for Linux gamers.</p>
    </footer>
  </div>
</template>
