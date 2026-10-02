<script setup>
function applyJob() {
  alert('Application started!')
}

defineProps({
  job: {
    type: Object,
    required: true
  }
})
</script>

<template>
  <article class="job-card">

    <div class="company-logo">
      {{ job.company.charAt(0) }}
    </div>

    <div class="job-content">

      <h3>
        {{ job.title }}
      </h3>

      <p class="company-name">
        {{ job.company }}
      </p>

      <p class="job-location">
        {{ job.location }} · {{ job.type }}
      </p>

    </div>
<button class="apply-button" @click="applyJob">
  Apply
</button>
  </article>
</template>

<style scoped>
.job-card {
  padding: 24px;
  border: 1px solid #e5e7eb;
  border-radius: 10px;
  background: #ffffff;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.job-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.06);
}

.company-logo {
  width: 44px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  border-radius: 8px;
  background: #f3f4f6;
  font-weight: 700;
}

.job-content h3 {
  margin: 0 0 8px;
  font-size: 18px;
}

.company-name {
  margin: 0 0 6px;
  color: #374151;
}

.job-location {
  margin: 0;
  color: #6b7280;
  font-size: 14px;
}

.apply-button {
  width: 100%;
  margin-top: 22px;
  padding: 11px;
  border: 1px solid #d1d5db;
  border-radius: 6px;
  background: #ffffff;
  cursor: pointer;
}

.apply-button:hover {
  background: #f9fafb;
}
</style>