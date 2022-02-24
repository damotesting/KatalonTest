# KatalonTest
var assert = require('assert');

describe('katalon', function() {

	it('should do something', function() {
		browser.url('https://www.google.com/');
		$('[name="q"]').setValue('yunex traffic');
		$('[name="btnI"]').click();
		browser.url('https://www.yunextraffic.com/global/en/');
		expect( $('//section[@id=\'c91\']/div/div/div/div/div/div/div/h2')).toHaveTextContaining(`Yunex Traffic: We launch cities into the future.`);
	});

});
