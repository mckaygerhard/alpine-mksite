<div class="pure-g">
   
    <div class="pure-u-1 pure-u-md-1-2">
        <div class="l-box">
            <h2>
                <a href="/atom.xml" class="atom"><i class="fa fa-rss"></i></a>
                Alpine News
            </h2>
            <ul class="home-list">
               {{#news}}
                <li><time>{{date}}</time>  <a href="posts/{{html}}">{{title}}</a></li>
               {{/news}}
            </ul>
            <a class="pure-button read-more" href="/posts">Read more</a>
        </div>

    </div>

    <div class="pure-u-1 pure-u-md-1-2">
        <div class="l-box">
            <h2>
                <a href="http://git.alpinelinux.org/cgit/aports" class="cgit">
                    <i class="fa fa-git "></i>
                </a>
                Latest development
            </h2>
            <ul class="home-list">
            {{#git-commits.entries}}
                <li><time datetime="{{updated}}">{{updated_date}}</time>  <a href="{{{link}}}">{{title}}</a></li>
            {{/git-commits.entries}}
            </ul>
            <a class="pure-button read-more" href="https://git.alpinelinux.org/cgit/aports/log">Read more</a>
        </div>
    </div>

</div> <!-- end pure-g -->