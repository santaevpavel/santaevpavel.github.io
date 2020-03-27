---
layout: post
title: "My first test post"
description: "My first test post with code."
category: articles
tags: [sample post, readability, test]
image:
  feature: "altai.jpg"
---


## Title


```kotlin
private fun initMetricProcessors() {
    logger.info("Loading metrics processors")
    processors = metricsProcessorsLoader.load(pluginClasspath.toCollection(mutableListOf()))
    processors?.collectors?.forEach { collector ->
        collector.init(metricsStore, project)
    }
    logCollectorsAndDispatchers()
    project.whenBuildFinished { dispatchMetrics() }
}
```

{: .language-kotlin}

{% highlight kotlin linenos %}
private fun initMetricProcessors() {
    // comment
    logger.info("Loading metrics processors")
    processors = metricsProcessorsLoader.load(pluginClasspath.toCollection(mutableListOf()))
    processors?.collectors?.forEach { collector ->
        collector.init(metricsStore, project)
    }
    logCollectorsAndDispatchers()
    project.whenBuildFinished { dispatchMetrics() }
}
{% endhighlight %}
