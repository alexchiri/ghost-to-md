---
title: ${post.title}<% if (post.slug) { %>
slug: ${post.slug}<% } %><%if (post.image) { %>
image: ${post.image}<% } %>
date_published: ${post.publishedAt}
date_updated:   ${post.updatedAt}<% if (post.tags.length) { %>
tags: ${post.tags.join(', ')}<% } %><% if (post.status === 'draft') { %>
draft: true<% } %>
---

${post.markdown}
