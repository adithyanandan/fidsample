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
