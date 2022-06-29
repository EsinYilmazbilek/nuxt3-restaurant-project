<template>
  <div>
    <Html :lang="dynamic > 50  ? 'en-GB' : 'eng-US'">
      <Head>
        <Title>Top 50 Restaurants</Title>
        <Meta 
          name="description"
          content="restaurant guide"
        />
        <Link 
          rel="preload" 
          href="https://www.iconpacks.net/icons/2/free-sad-face-icon-2691-thumb.png"
          as="script"
        />
      </Head>
    </Html>

    <NuxtLayout name="custom">
      <div class="container">
        <RestaurantTable />
      </div>
    </NuxtLayout>
  </div>
</template>
