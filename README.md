# 所有文章
<div style="display: flex; flex-direction: column">
    <div v-for="page of $site.pages.filter(item => item.path !== '/')" :key="page.key" style="padding: 20px 0; max-width: 33%;">
        <router-link :to="page.path">
            {{page.title}}
            <div style="color: #c2c5cd; font-size: .5rem;">{{(page.frontmatter.tags || ['无标签']).join(',  ')}}</div>
        </router-link>
    </div>
</div>

作者：Mizuka
链接：https://www.jianshu.com/p/03ce29b7f633
來源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。
