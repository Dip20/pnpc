<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
<script src="push.min.js"></script>
<script src="serviceWorker.min.js"></script>
<script>
function start(){
	Push.create("Hello world!", {
		body: "How's it hangin'?",
		icon: 'https://previews.123rf.com/images/coolvectorstock/coolvectorstock1808/coolvectorstock180802556/106911764-blood-sample-vector-icon-isolated-on-transparent-background-blood-sample-logo-concept.jpg',
		timeout: 4000,
		onClick: function () {
			window.focus();
			this.close();
		}
	});
}

function clear(){
	Push.clear();
}
</script>
<a href="javascript:void(0)" onclick="start()">Start</a>
<a href="javascript:void(0)" onclick="clear()">Clear</a>
