# fidsample
import java.util.List;

public class Payload {
    private List<Data> data;

    public List<Data> getData() {
        return data;
    }

    public void setData(List<Data> data) {
        this.data = data;
    }

    public static class Data {
        private String contentId;
        private String population;
        private String reminderFlag;

        public String getContentId() {
            return contentId;
        }

        public void setContentId(String contentId) {
            this.contentId = contentId;
        }

        public String getPopulation() {
            return population;
        }

        public void setPopulation(String population) {
            this.population = population;
        }

        public String getReminderFlag() {
            return reminderFlag;
        }

        public void setReminderFlag(String reminderFlag) {
            this.reminderFlag = reminderFlag;
        }
    }
}
import com.fasterxml.jackson.core.JsonProcessingException;
import com.fasterxml.jackson.databind.ObjectMapper;

public class Main {
    public static void main(String[] args) {
        // Create the object
        Payload payload = new Payload();
        Payload.Data data = new Payload.Data();
        data.setContentId("Test_Email");
        data.setPopulation("Dynamic");
        data.setReminderFlag("N");

        // Add the data to the list in payload
        payload.getData().add(data);

        // Convert the object to JSON
        ObjectMapper objectMapper = new ObjectMapper();
        String jsonPayload;
        try {
            jsonPayload = objectMapper.writeValueAsString(payload);
            // Print or send jsonPayload to the front end
            System.out.println(jsonPayload);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
        }
    }
}



 "contentIdLists": [
            {
                "entries": [
                    {
                        "contentId": "Test_Email",
                        "population": "Dynamic",
                        "reminderFlag": "N"
                    },
                    {
                       
                      "contentId": "Test_Email",
                        "population": "Dynamic",
                        "reminderFlag": "N"
                    }
                     ]
            }
        ]![image](https://github.com/adithyanandan/fidsample/assets/28766388/2e0467c5-e3e5-4101-90f2-9417243e37c0


        $scope.contentIdLists = [
          {
            entries: [
              {
                contentId: "Test_Email",
                population: "Dynamic",
                reminderFlag: "N"
              },
              {
                contentId: "Test_Email_2",
                population: "Dynamic",
                reminderFlag: "N"
              }
            ]
          }
        ];

        "<jqx-combo-box id='populateEx' ng-disabled=\"$ctrl.disabledFields\" remove-model ng-model=\"$ctrl.populationOptEx\" ng-disabled=' $ctrl.disabledFields'" +
			"jqx-settings=\"populationSettingsEx\" jqx-on-close=\"changeHandler_POPULATIONINDEx(event)\" style=\"margin-top: 5px;\" spark-change-data></jqx-combo-box>" +

			"</div>" +
			"<div class=\"col-sm-1 deleteIcon\">" +
			"<a href=\"\" ng-disabled=\"$ctrl.disabledFields\"ng-class=\"{disabled: $ctrl.disabledFields}\" ng-click=\"$ctrl.deleteComponentEx($event,'populationOptEx',5)\"> <span class=\"glyphicon glyphicon-trash\"></span></a>" +
			"</div>";

	$ctrl.population = "<div class=\"col-sm-6 alignRecepient\">" +
			"<jqx-combo-box id='populate'ng-disabled=\"$ctrl.disabledFields\" remove-model ng-model=\"$ctrl.populationOpt\" ng-disabled=' $ctrl.disabledFields'" +
			"jqx-settings=\"populationSettings\" jqx-on-close=\"changeHandler_POPULATIONIND(event)\" style=\"margin-top: 5px;\" spark-change-data></jqx-combo-box>" +

			"</div>" +
			"<div class=\"col-sm-1 deleteIcon\">" +
			"<a href=\"\" ng-disabled=\"$ctrl.disabledFields\" ng-class=\"{disabled: $ctrl.disabledFields}\" ng-click=\"$ctrl.deleteComponent($event,'populationOpt',7)\"> <span class=\"glyphicon glyphicon-trash\"></span></a>" +
			"</div>";
   ![image](https://github.com/adithyanandan/fidsample/assets/28766388/3fdd215f-eb14-4a96-85a0-3f0907eb6277)

   $ctrl.changeHandler_POPULATIONIND = function (event) {
    // Check if 'US' is selected
    if ($ctrl.populationOpt === 'US') {
        // Display additional fields 'ES' and 'NONES'
        $ctrl.additionalFields = ['ES', 'NONES'];
    } else {
        // Hide additional fields for other options
        $ctrl.additionalFields = [];
    }
};
jqx-on-change=\"$ctrl.changeHandler_POPULATIONIND(event)\" jqx-on-close=\"$ctrl.closeHandler_POPULATIONIND(event)\"

 $scope.populationSettings = {
			   source: populationOptions,
			   showArrow: true,
			   multiSelect: true,
			   width: '95%',
			   height: 25,
			   checkboxes: true,
			   created: function (args) {
				   $scope.pop_Opt = args.instance;
				   checkCombo($scope.pop_Opt, $ctrl.populationOpt);
			   }
		   };

     Resilience and Hard Work: The film highlights the dedication and resilience of the McFarland cross country team. Despite numerous obstacles and limited resources, the students commit themselves to intense training and work hard to achieve success.
Community and Family: "McFarland, USA" shows the importance of community support and the strength of family bonds. The coach learns to understand and appreciate the town's culture, and the team becomes like a family, supporting each other through challenges.
Overcoming Prejudice: The film addresses themes of prejudice and cultural differences, showing how the coach and the students navigate and overcome stereotypes. The transformation of the coach's perspective on the Latino community is a key aspect of the story.
Empowerment and Opportunity: By participating in cross country, the students discover new opportunities and pathways to success. The film emphasizes the potential for sports to empower individuals and provide them with life-changing experiences.
Teamwork and Leadership: The development of teamwork and leadership skills is a central theme. Coach White's guidance and the team's collective effort demonstrate that great things can be achieved when people work together.
Cultural Identity and Heritage: The film acknowledges the cultural identity of the students and shows how they embrace their heritage while striving for excellence in cross country. It promotes pride in one's background and the idea that cultural differences can be strengths rather than obstacles.


<dependency>
    <groupId>jakarta.xml.soap</groupId>
    <artifactId>jakarta.xml.soap-api</artifactId>
    <version>2.0.0</version>
</dependency>
<dependency>
    <groupId>com.sun.xml.messaging.saaj</groupId>
    <artifactId>saaj-impl</artifactId>
    <version>2.0.1</version>
</dependency>


function replacePlaceholders(template, values) {
  // Extract placeholders from the template string
  let regex = /%%(.*?)%%/g;
  let match;
  let placeholders = [];

  // Find all placeholders in the template
  while ((match = regex.exec(template)) !== null) {
    placeholders.push(match[1]);
  }

  // Replace placeholders with corresponding values
  placeholders.forEach(placeholder => {
    if (values[placeholder]) {
      template = template.replace(new RegExp(`%%${placeholder}%%`, 'g'), values[placeholder]);
    }
  });

  return template;
}

// Example usage
let template = "Your %%Product_Type%% will expire on %%Date_from%% to the percent %%DATE_TO%%";
let values = {
  Product_Type: "Subscription",
  Date_from: "2024-05-22",
  DATE_TO: "2024-06-22"
};

let result = replacePlaceholders(template, values);
console.log(result); // Output: "Your Subscription will expire on 2024-05-22 to the percent 2024-06-22"

$scope.startRegex = '%%.*_START_DATE%%';
							$scope.endRegex = '%%.*_END_DATE%%'
							$scope.prodRegex='%%PI_PRODUCT_TYPE%%';
							$scope.shareRegex='%%PI_PROCEED_TYPE%%';
							$scope.taxMethodRegex ='%%PI_TAX_METHOD%%';


$ctrl.parseDate = function (data) {
			data = data || '';
				
					$ctrl.messageDetails = data;
				
			data = data.replace(/<date>/g, '').replace(/<\/date>/g, '');
			var tempUs = '';
			
				if (data.match($ctrl.startRegex) && data.match($ctrl.endRegex)) {
					var startDate = data.match($ctrl.startRegex)[0];
					$ctrl.messageDetails = data.replace(startDate, '01/01/2017');
					var endDate = $ctrl.messageDetails.match($ctrl.endRegex)[0];
					$ctrl.messageDetails = $ctrl.messageDetails.replace(endDate, '12/31/2017');
				} else if (data.match($ctrl.startRegex) && !data.match($ctrl.esharendRegex)) {
					tempUs = data.match($ctrl.startRegex)[0];
					$ctrl.messageDetails = data.replace(tempUs, '01/01/2017');
				} else if (data.match($ctrl.endRegex) && !data.match($ctrl.startRegex)) {
					tempUs = data.match($ctrl.endRegex)[0];
					$ctrl.messageDetails = data.replace(tempUs, '12/31/2017');
				} else if (data.match($ctrl.prodRegex)) {
					$ctrl.messageDetails = data.replace($ctrl.prodRegex, 'PRODUCT(S)');
				} else if (data.match($ctrl.shareRegex)) {
					$ctrl.messageDetails = data.replace($ctrl.shareRegex, 'SHARES/PROCEEDS');
				} else if (data.match($ctrl.taxMethodRegex)) {
					$ctrl.messageDetails = data.replace($ctrl.taxMethodRegex, 'TAX METHOD');
				}
			
		}
<div style="margin: 10px 0px 10px 0px;" ng-if="($ctrl.templateTypeCode == 'D' || $ctrl.templateTypeCode == 'F')">
				<label class="font-thin">Broker Name&nbsp;</label>  <select ng-model="$ctrl.alertConfig.brokerNameNewCnt" ng-options="c for c in brokerNameNewCnt"></select>
			</div>
   if (row.variableName == 'PI_BROKER_NAME'){
                                            $scope.brokerNameNewCnt = row.variableValues.split(',');
                                            $ctrl.alertConfig.brokerNameNewCnt = row.labelName;
                                        } // FI,FIL

     // modified
     <div style="margin: 10px 0px 10px 0px;" ng-if="($ctrl.templateTypeCode == 'D' || $ctrl.templateTypeCode == 'F')">
    <label class="font-thin">Broker Name&nbsp;</label>
    <select ng-model="$ctrl.alertConfig.brokerNameNewCnt" ng-options="c for c in filteredBrokerNameNewCnt"></select>
</div>

if (row.variableName == 'PI_BROKER_NAME') {
    let allBrokerNames = row.variableValues.split(',');
    
    // Assuming you have a filter condition variable
    let filterCondition = 'US'; // Replace this with the actual condition check
    
    if (filterCondition == 'US') {
        $scope.filteredBrokerNameNewCnt = allBrokerNames.filter(function(name) {
            return name === 'FI';
        });
    } else {
        $scope.filteredBrokerNameNewCnt = allBrokerNames;
    }
    
    $ctrl.alertConfig.brokerNameNewCnt = row.labelName;
}

SELECT count(1)
                                 FROM alrt_prsr_prtc app
                                 JOIN alrt_prsr_prtc_dtl appd ON (app.alrt_prsr_prtc_id = appd.alrt_prsr_prtc_id)
                                WHERE pi.plan_sponsor_id = app.plan_sponsor_id
                                  AND pi.participant_id = app.participant_id
                                  AND to_char(pi.PRTC_GRANT_ID) = app.grant_id
                                  AND app.ALRT_CHN_ID = g_alrt_chn_id
                                  AND appd.stat_c != 'M' and rownum=1) > 0



        INSERT INTO alrt_prsr_prtc(ALRT_PRSR_PRTC_ID, ALRT_PRSR_MST_ID, PLAN_SPONSOR_ID, CLNT_PKG_ID, CLNT_ALRT_CNFG_ID,
                             PARTICIPANT_ID, TMPL_APLC_TO, ALRT_VAR_VAL,
                             PRCS_D, INSERT_D, INSERT_USER, LST_UPD_D, LST_UPD_USER, ALRT_CHN_ID)
  WITH grants AS
                (
                SELECT distinct
                    gpl.plan_sponsor_id, gpl.participant_id, gpl.tmpl_aplc_to,
    CASE when product_ty_c = 'RU' and NVL(pln.perf_awrd_i,'N') = 'N' then 'RSU'
    when product_ty_c = 'RU' and NVL(pln.perf_awrd_i,'N') = 'Y' then 'PA'
    ELSE product_ty_c
    END product_ty_c ,
    CASE WHEN rsu_proc_ty_c = 'S' THEN 'SHARES'
    ELSE 'CASH'
    END PROCTYPCODE
    FROM gt_participant_list gpl
    join participant_ra_trade prat on (gpl.plan_sponsor_id = prat.plan_sponsor_id and
	                                   gpl.participant_id = prat.participant_id and
									   prat.logical_delete_i='N')
    join product pdct ON (prat.plan_sponsor_id = pdct.plan_sponsor_id and prat.product_id = pdct.product_id and
	                      pdct.logical_delete_i = 'N')
    join plan pln ON (pdct.plan_sponsor_id = pln.plan_sponsor_id and pdct.plan_id = pln.plan_id and
	                  pln.logical_delete_i = 'N')

    WHERE (((prat.tax_wh_meth_c IS NULL OR prat.tax_wh_meth_c <> 'S') AND trunc(prat.trx_d) = trunc(l_ref_date)) OR
          (prat.tax_wh_meth_c = 'S' AND trunc(prat.trx_d) = trunc(l_stc_date)))
      AND prat.rec_ty_c IN ('V', 'S')
      and (prat.exec_stat_c is null or prat.exec_stat_c != 'C')
      AND (prat.shr_dep_a > 0 OR prat.net_csh_proc_rsu_a > 0)
      and ((prat.rsu_proc_ty_c = 'C' and prat.jrnl_ty_c ='F')
	    OR (prat.rsu_proc_ty_c = 'S' and sale_avl_d IS NULL AND (prat.jrnl_ty_c IS NULL OR prat.jrnl_ty_c ='F')))
	  AND prat.src_system_id = 1 --legacy grants
   )
        SELECT SEQ_ALRT_PRSR_PRTC_ID.NEXTVAL, g_alrt_prsr_mst_id, g_plan_sponsor_id, g_clnt_pkg_id, g_clnt_alrt_config_id,
        participant_id, tmpl_aplc_to, 'PI_PRODUCT_TYPE='||NVL(cdn.dyn_nm , cdn2.dyn_nm)||';PI_PROCEED_TYPE='||PROCTYPCODE,
        SYSDATE, SYSDATE, g_user, NULL, NULL, g_alrt_chn_id
        from grants

    LEFT JOIN clnt_dyn_nm cdn ON (grants.plan_sponsor_id = cdn.plan_sponsor_id AND
                                  grants.product_ty_c = cdn.itrn_nm AND
                                  cdn.appl_ty_c = 'PRDT_NM')
    JOIN clnt_dyn_nm cdn2 ON (cdn2.plan_sponsor_id = 0 AND
                              grants.product_ty_c = cdn2.itrn_nm AND
                              cdn2.appl_ty_c = 'PRDT_NM');

 END LOOP;

 SELECT distinct
                    gpl.plan_sponsor_id, gpl.participant_id, gpl.tmpl_aplc_to,
    CASE when product_ty_c = 'RU' and (pln.CSH_PLAN_I = 'T') then 'cash'
         when product_ty_c = 'RU' and (pln.CSH_PLAN_I = 'P') then 'performance-based cash'
         when product_ty_c = 'RU' and NVL(pln.perf_awrd_i,'N') = 'N' then 'RSU'
    when product_ty_c = 'RU' and NVL(pln.perf_awrd_i,'N') = 'Y' then 'PA'
    ELSE product_ty_c
    END product_ty_c ,
    CASE WHEN rsu_proc_ty_c = 'S' THEN 'SHARES'
    ELSE 'CASH'
    END PROCTYPCODE
    FROM gt_participant_list gpl

    You can do that way more efficiently by nesting logic under product_ty_c = 'RU' rather than having cases that check that field four separate times
Your logic to set RSU and PA also applies to Cash, so even if this did compile, everything would still end up RSU and PA


   MERGE INTO alrt_prsr_prtc_web_msg appwm
  USING
  (
   WITH  A AS
        (
          SELECT  ggpl.plan_sponsor_id,ggpl.participant_id,awd.grant_tranche_id, ggpl.tmpl_aplc_to,pdct.src_product_id, pag.sub_product_ty_c,
           Pag.Grant_D, Ltrim(Lpad(Substr(Pag.Seq_N,Length(Pag.Seq_N)-2,3),3,0),'0 ') As Seq_N, Pag.Grant_Id, Pln.Src_Plan_Id,Pln.Tsru_I,Pln.CSH_PLAN_I,Pln.Perf_Awrd_I,
           Case When Pdct.Product_Ty_C = 'RU' and (pln.CSH_PLAN_I = 'T') then 'CSH'
                 When Pdct.Product_Ty_C = 'RU' and (pln.CSH_PLAN_I = 'P') then 'PC'
                    When Pdct.Product_Ty_C = 'RU' And Nvl(Pln.Perf_Awrd_I,'N') = 'N' And Nvl(Pln.Tsru_I,'N') = 'N' Then 'RSU'
                        When Pdct.Product_Ty_C = 'RU' And Nvl(Pln.Perf_Awrd_I,'N') = 'Y' And Nvl(Pln.Tsru_I,'N') = 'N' Then 'PA'
	                        When Pdct.Product_Ty_C = 'RU' And Nvl(Pln.Tsru_I,'N')='Y' Then 'TSRU'
    ELSE pdct.product_ty_c
    END product_ty_c , NVL(pag.tax_wh_meth_c, pdct.tax_wh_meth_c) tax_wh_meth_c, NVL(pag.tax_wh_def_c, pdct.tax_wh_def_c) tax_wh_def_c, awd.pay_d,
	case when ps.RLUP_PLN_I = 'Y' then '' else pln.src_plan_id end drv_pln_id
          FROM gt_grant_participant_list ggpl
            JOIN plan_sponsor ps ON (ggpl.plan_sponsor_id = ps.plan_sponsor_id)
            JOIN participant_award_grant pag ON (ggpl.plan_sponsor_id = pag.plan_sponsor_id AND
                                                ggpl.participant_id = pag.participant_id AND
                                                ggpl.grant_id=pag.grant_id AND
                                                pag.logical_delete_i = 'N')
            JOIN grant_tranche gt ON (pag.plan_sponsor_id = gt.plan_sponsor_id AND
                                       pag.grant_id = gt.grant_id AND
                                       gt.logical_delete_i = 'N')
            JOIN award_distribution awd ON(pag.plan_sponsor_id = awd.plan_sponsor_id AND
                                            gt.grant_tranche_id = awd.grant_tranche_id AND
                                            awd.logical_delete_i = 'N')
			JOIN participant_detail pd ON(ggpl.plan_sponsor_id=pd.plan_sponsor_id AND
                                          ggpl.participant_id = pd.participant_id)
            JOIN product pdct ON (pag.plan_sponsor_id = pdct.plan_sponsor_id AND
                                  pag.product_id = pdct.product_id AND
                                  pdct.logical_delete_i = 'N')
            JOIN plan pln ON (ggpl.plan_sponsor_id = pln.plan_sponsor_id AND
                               pdct.plan_id = pln.plan_id AND
                               pln.logical_delete_i = 'N')
            LEFT JOIN grant_agreement gag ON (pag.plan_sponsor_id=gag.plan_sponsor_id AND
                                             pag.grant_id = gag.grant_id AND
                                             gag.logical_delete_i = 'N')
            JOIN grant_status gs ON (pag.plan_sponsor_id = gs.plan_sponsor_id AND
                                  pag.product_id = gs.product_id AND
                                  pag.sub_product_ty_c = gs.sub_product_ty_c AND
                                  pag.grant_d = gs.grant_d AND
                                  gs.seq_n = CASE WHEN ps.admin_ty_c = 'PA' THEN 1 ELSE pag.seq_n END AND
                                  gs.logical_delete_i = 'N')

         WHERE awd.pay_d between rec.start_date AND rec.end_date AND (awd.admin_only_c != 'D' OR awd.admin_only_c is NULL)
           AND awd.dist_stat_c = 'P'
           AND gt.shr_tot_a <> shr_cncl_a and gt.shr_exercisable_a > 0 and (gt.shr_cncl_d > l_ref_date OR gt.shr_cncl_d IS NULL)
           AND pd.enrl_rsu_i='Y'  AND pd.wh_tax_i='Y'
           AND (pd.admin_only_c IS NULL OR pd.admin_only_c='N')
           AND (pag.cancel_d is null or pag.cancel_d > l_ref_date)
           AND pag.shr_granted_a <> pag.shr_exer_a
           AND pag.opt_ostd_a > 0
           AND pag.sub_product_ty_c IN('RSU')
           AND coalesce(pag.tax_wh_def_c,pdct.tax_wh_def_c) IN ('C','N','S')
           AND coalesce(pag.tax_wh_meth_c,pdct.tax_wh_meth_c) IN ('B','A','M','O','N','C','S')
           AND (pag.byp_tx_calc_i IS NULL OR pag.byp_tx_calc_i ='N')
           AND (pdct.oga_svc_i IS NULL OR pdct.oga_svc_i = 'N' OR ((pdct.oga_svc_i = 'Y' OR pdct.oga_svc_i = 'C') AND pag.acp_dcln_c = 'A'))
	       AND (pdct.oga_svc_i IS NULL OR pdct.oga_svc_i = 'N' OR ((pdct.oga_svc_i = 'Y' OR pdct.oga_svc_i = 'C') AND gag.acp_dcln_i= 'A'))
           AND (pln.pub_client_i='Y' OR (pln.pub_client_i='N' and COALESCE(pdct.shr_proc_i,'N') ='N'))
           AND pdct.product_ty_c IN('RU')
           AND gs.grant_stat_c = 'A'
           AND (gs.web_trading_i = 'Y' OR gs.rep_trading_i = 'Y' OR gs.wireless_trading_i = 'Y' OR gs.phone_trading_i = 'Y')
           AND pag.plan_sponsor_id = g_plan_sponsor_id and pag.src_system_id = 1 -- MF Grants

       ),
       b AS
           (
             SELECT grant_id, grant_tranche_id, plan_sponsor_id, tax_meth_elct_c,
             'PI_PROD_ID='||src_product_id||';PI_SUB_PROD_TY_CD='||sub_product_ty_c||
            ';PI_GRANT_DATE='||to_char(grant_d,'YYYY-MM-DD')||';PI_GRANT_SEQ_NUM='||seq_n||
            ';PI_GRANT_ID='||grant_id||
            ';PI_PLAN_ID='||drv_pln_id||
            ';PI_PLAN_TY_C='||
            CASE WHEN sub_product_ty_c IN ('RSU') AND NVL(tsru_i,'N')='Y' THEN 'T'
                WHEN sub_product_ty_c IN ('RSU') AND NVL(perf_awrd_i,'N') = 'Y' AND NVL(tsru_i,'N') = 'N' THEN 'E'
                WHEN sub_product_ty_c IN ('RSU') AND  NVL(perf_awrd_i,'N') = 'N' AND NVL(tsru_i,'N') ='N' THEN 'N'
            END||
           ';PI_PRODUCT_TYPE='||product_ty_c||
           ';PI_RESTRICTED_RELEASE_DATE='||to_char(pay_d,'fmMonth DD, YYYY')||
           ';PI_TAX_METHOD_CHOICE='||
           CASE WHEN tax_wh_meth_c IN('B','A','M','O') THEN 'CHOICE' ELSE 'NOCHOICE' END ||
           ';PI_TAX_METHOD='||
           CASE WHEN tax_wh_meth_c IN('B','A','M','O') AND COALESCE(tax_meth_elct_c, tax_wh_def_c ,tax_wh_meth_c)='N' THEN 'Net Shares'
                WHEN tax_wh_meth_c IN('B','A','M','O') AND COALESCE(tax_meth_elct_c, tax_wh_def_c ,tax_wh_meth_c)='S' THEN 'Sell Shares'
                WHEN tax_wh_meth_c IN('B','A','M','O') AND COALESCE(tax_meth_elct_c, tax_wh_def_c ,tax_wh_meth_c)='C' THEN 'Deposit Funds'
								WHEN COALESCE(tax_wh_def_c ,tax_wh_meth_c)='N' THEN 'Net Shares'
                WHEN COALESCE(tax_wh_def_c ,tax_wh_meth_c)='S' THEN 'Sell Shares'
                WHEN COALESCE(tax_wh_def_c ,tax_wh_meth_c)='C' THEN 'Deposit Funds'
           END || ';PI_PARTICIPANT_ID='||participant_id  alrt_var_val ,
           ROW_NUMBER() OVER(PARTITION BY participant_id,drv_pln_id,(Case When Product_Ty_C = 'RU' and (CSH_PLAN_I = 'T') then 'CSH'
            When Product_Ty_C = 'RU' and (CSH_PLAN_I = 'P') then 'PC'
                When Product_Ty_C = 'RU' And Nvl(Perf_Awrd_I,'N') = 'N' And Nvl(Tsru_I,'N') = 'N' Then 'RSU'
			        When Product_Ty_C = 'RU' And Nvl(Perf_Awrd_I,'N') = 'Y' And Nvl(Tsru_I,'N') = 'N' Then 'PA'
			When Product_Ty_C = 'RU' And Nvl(Tsru_I,'N')='Y' Then 'TSRU'
			ELSE product_ty_c END) , pay_d,
            (CASE WHEN tax_wh_meth_c IN ('B','A','M','O') THEN 'CHOICE' ELSE 'NOCHOICE' END),
            (CASE WHEN tax_wh_meth_c IN('B','A','M','O') AND COALESCE(tax_meth_elct_c, tax_wh_def_c ,tax_wh_meth_c)='N' THEN 'Net Shares'
                WHEN tax_wh_meth_c IN('B','A','M','O') AND COALESCE(tax_meth_elct_c, tax_wh_def_c ,tax_wh_meth_c)='S' THEN 'Sell Shares'
                WHEN tax_wh_meth_c IN('B','A','M','O') AND COALESCE(tax_meth_elct_c, tax_wh_def_c ,tax_wh_meth_c)='C' THEN 'Deposit Funds'
								WHEN COALESCE(tax_wh_def_c ,tax_wh_meth_c)='N' THEN 'Net Shares'
                WHEN COALESCE(tax_wh_def_c ,tax_wh_meth_c)='S' THEN 'Sell Shares'
                WHEN COALESCE(tax_wh_def_c ,tax_wh_meth_c)='C' THEN 'Deposit Funds'
            END)  ORDER BY grant_id) bundle_rnk,
           tmpl_aplc_to,participant_id
           FROM (
                     SELECT src_plan_id, src_product_id, seq_n, sub_product_ty_c,  grant_d, th.tax_meth_elct_c,a.participant_id ,a.grant_tranche_id,a.grant_id,a.tax_wh_def_c,a.tax_wh_meth_c,a.plan_sponsor_id,a.tmpl_aplc_to,
                    ROW_NUMBER() OVER(PARTITION BY A.participant_id, A.grant_tranche_id, A.plan_sponsor_id ORDER BY th.upd_tmst DESC) as rnk, NVL(cdn.dyn_nm , cdn2.dyn_nm) product_ty_c, pay_d, tsru_i, perf_awrd_i,  drv_pln_id
                 From  A Left Join Participant_Tax_Meth Th On(A.Plan_Sponsor_Id = Th.Plan_Sponsor_Id And
                                              a.grant_tranche_id = th.grant_tranche_id)
                                             LEFT JOIN clnt_dyn_nm cdn ON (a.plan_sponsor_id = cdn.plan_sponsor_id AND
                                  a.product_ty_c = cdn.itrn_nm AND
                                  cdn.appl_ty_c = 'PRDT_NM')
            JOIN clnt_dyn_nm cdn2 ON (cdn2.plan_sponsor_id = 0 AND
                              A.Product_Ty_C = Cdn2.Itrn_Nm And
                              cdn2.appl_ty_c = 'PRDT_NM' )where th.tax_meth_elct_c is null or th.tax_meth_elct_c IN ('C','N','S')) s
                        WHERE s.rnk = 1
      )
	   SELECT distinct  b.plan_sponsor_id , b.participant_id, b.tmpl_aplc_to, b.alrt_var_val, g_message_id message_id
            from b where bundle_rnk =1
    ) upd
     ON (appwm.plan_sponsor_id = upd.plan_sponsor_id AND
         appwm.participant_id = upd.participant_id AND
         appwm.alrt_var_val = upd.alrt_var_val AND
         appwm.message_id = upd.message_id)
   WHEN MATCHED THEN
        UPDATE SET eff_end_dt = to_timestamp(to_char (sysdate+1, 'dd-mm-YYYY') || '080000.00', 'dd-mm-YYYYhh24miss.ff'),
                   logical_delete_i = 'N',
                   lst_upd_d = SYSDATE,
                   lst_upd_user = user;
    END LOOP;
  END IF;
END IF;

10174/4  PL/SQL: SQL Statement ignored                                          
10265/43 PL/SQL: ORA-00904: "CSH_PLAN_I": invalid identifier   

