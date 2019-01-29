/** 
 * Cria pixel contador para enviar dados da matéria para o STATS
 *
 * Date: Fri Jan 18 2013 19:08:15 GMT-0300
 */

( function () {

var stats = {
	url: "//stats1.folha.uol.com.br/stats" ,
	old_url: "//stats.folha.uol.com.br/stats" ,

	random: function ( n ) {
		var min , max ;
		n = n || 10 ;
		min = Math.pow( 10, n - 1 ) ;
		max = Math.pow( 10, n ) - 1 ;

		return Math.round( Math.random() * ( max - min ) + min ) ;
	} ,

	init: function () {
		var base = this, article_url = [location.protocol, "//", location.host, location.pathname].join("") ;
		document.write( '<img src="' + base.url + '?url=' + escape( article_url ) + '&amp;ref=' + escape( document.referrer || '' ) + '&amp;rand=' + base.random() + '" width="1" height="1" alt="">' ) ;
	}
} ;

stats.init() ;

} )( window ) ;