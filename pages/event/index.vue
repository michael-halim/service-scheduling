<template>
  <div class="container my-3">
    <div class="card">
      <div class="card-body">
        <table class="table">
          <thead>
            <tr>
              <th>Visibility</th>
              <th>Event Date Start</th>
              <th>Event Date End</th>
              <th>Event Name</th>
              <th>Event Owner</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Icon</td>
              <td>
                <nuxt-link :to="'/event/event-detail'" class="nav-link">
                  7/21/2022 08:00
                </nuxt-link>
              </td>
              <td>
                <nuxt-link :to="'/event/event-detail'" class="nav-link">
                  7/21/2022 08:00
                </nuxt-link>
              </td>
              <td>
                <nuxt-link :to="'/event/event-detail'" class="nav-link">
                  Ibadah
                </nuxt-link>
              </td>
              <td>
                <nuxt-link :to="'/event/event-detail'" class="nav-link">
                  Yunus
                </nuxt-link>
              </td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style scoped>
</style>
