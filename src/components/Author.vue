<template>
  <div style="display: contents">
    <g-link to="/">
      <g-image
        src="~/assets/img/profile2.png"
        :alt="$static.metadata.siteName"
      ></g-image>
    </g-link>
    <h1>
      <a href="/">Personal Blog of Jonas Doe</a>
    </h1>

    <p>Get to know the coolest trends in dev</p>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
	siteDescription
  }
}
</static-query>

<script>
export default {
  props: ["showTitle"],
};
</script>
