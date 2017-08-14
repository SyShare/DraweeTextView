# DraweeTextView 援引：https://github.com/Bilibili/drawee-text-view.git
对于bibili分享的DraweeText进一步定制，可使图文居中对齐


DraweeTextView textview = (DraweeTextView)findViewById(R.id.text);

SpannableStringBuilder builder = new SpannableStringBuilder();
builder.append("2333333\n")
start = builder.length();
builder.append("[emotion:tv_cheers]");
DraweeSpan span = new DraweeSpan("http://static.yo9.com/web/emotions/tv_cheers.png");
builder.setSpan(span, start, builder.length(), Spanned.SPAN_EXCLUSIVE_EXCLUSIVE);
builder.append("bilibili- ( ゜- ゜)つロ 乾杯~\n");

...

textview.setText(builder);
